# Schallern Founder Collection: Reveal Rule (v1)

This document is the complete and binding rule for assigning artworks to Schallern Founder NFTs. It is published before the public mint opens (11 Nov 2026, 10:11 UTC). After that, it does not change. The SHA-256 hash of this file's exact bytes is published with the commit that adds it. Anyone can check every step below against public Solana data, with no help from the operator.

All parameters are in the machine-readable block below. The reference verifier (`scripts/reveal_verify.mjs`) reads its parameters from this block only. It never takes them from operator configuration or from the mint API.

<!-- RULE-PARAMS-BEGIN -->
```json
{
 "ruleVersion": 1,
 "cluster": "mainnet-beta",
 "candyMachine": "DSdMVfnsLzLev1yavmZ1SyqTUmgZyP4eTX9EpbjwvoC",
 "candyGuard": "4XAQYnGHtgg2jzueDRHQhw3SsZufmpuJnBGBgUiDxfc5",
 "collection": "GxNLJ6L13aY5NkyqPeQmzcvgBvssZkdxorzHY5zat4cE",
 "itemsAvailable": 10000,
 "namePrefix": "Schallern Founder #",
 "provenanceHash": "43f5bf16e59b3540ef2392f005de26cdd923d039825c632b0573a728171502cf",
 "offsetSlots": 300,
 "mintEnd": "2027-01-31T22:59:00Z",
 "commitment": "finalized",
 "programs": {
  "candyMachineCore": "CMACYFENjoBMHzapRXyo1JZkVS6EtaDDzkjMrmQLvr4J",
  "candyGuard": "CMAGAKJ67e9hRZgfC5SFTbZH8MgEmtqazKXjmkaJjWTJ",
  "mplCore": "CoREENxT6tW1HoK8ypY1SxRMZTcVPm7R94rH4PZNhX7d"
 },
 "mintAssetDiscriminator": "54afd39c38fa6876"
}
```
<!-- RULE-PARAMS-END -->

Notation: `N = itemsAvailable`. `sha256(x)` is the lowercase hex SHA-256 of the UTF-8 bytes of `x`. All chain reads use `finalized` commitment.

## 1. Pre-mint commitment (provenance)

1. Artworks are numbered `art = 1..N`. For each artwork there is one provenance line `art:sha256(image file bytes):sha256(canonical traits)`, in art order. The canonical traits are `JSON.stringify([art, seed, tier, material, finish, edge, motif, inscription, backdrop.plate || backdrop.wall, effect])`, taken from that artwork's entry in `collection.json`.
2. `provenanceHash = sha256(lines.join("\n") + "\n")`.
3. Before the first mint, `provenanceHash` is stored on-chain as the 32-byte `hash` of the Candy Machine's hidden settings. Every asset is minted with the same placeholder URI. The artworks, their order and the images are fixed by this hash and cannot change afterwards.

## 2. Founder number `#k` (mint-time index)

1. The Candy Machine uses hidden settings named `Schallern Founder #$ID+1$`. During each mint, the Candy Machine program creates the asset through an mpl-core `Create` instruction named `Schallern Founder #k`, where `k = itemsRedeemed + 1` at that moment. So `k` is the 1-based position of that mint in the Candy Machine's mint order.
2. A **mint transaction** is a successful finalized transaction (`meta.err = null`) that contains, at any stack height, both of these instructions:
   - an instruction of program `candyMachineCore` whose first 8 data bytes are `mintAssetDiscriminator` and whose account 0 is `candyMachine`; its account 5 is the asset and its account 6 must be `collection`;
   - an instruction of program `mplCore` with data byte 0 equal to `0` (CreateV1) or `20` (CreateV2), whose account 0 is that asset and whose account 1 is `collection`. Its `name` field must be `namePrefix + k`, with `k` a positive integer without leading zeros.
3. An asset's `k` comes **only** from its mint transaction. The asset's current on-chain name or URI never determines `k`.
4. The set of mint transactions comes from `getSignaturesForAddress(candyMachine)`, fully paginated. Any transaction that is not a mint transaction is ignored, even if it lists the Candy Machine as an account.
5. Let `S` be `itemsRedeemed` read from the Candy Machine account at reveal time. The mint set is valid only if the mint-time indices are exactly `{1, …, S}`, each appears once, each belongs to a different asset, and slots never decrease from `k` to `k + 1`. The collection must contain no asset other than these `S` minted assets.

## 3. Anchor slot `A`

- **Sold out (`S = N`):** `A` is the slot of the mint transaction with `k = N`. This is the mint that moved `itemsRedeemed` to `N`, and no mint transaction may have a later slot. No other transaction affects `A`, including any later transaction that touches the Candy Machine.
- **Not sold out (`S < N`):** the reveal happens only after `mintEnd`, and at least one asset must have been minted (`S ≥ 1`). Take the `endDate` of the Candy Guard's default guard set from the chain at reveal time. It must equal `mintEnd`; otherwise the reveal is invalid. `A` is the smallest produced (non-skipped) finalized slot whose block time is `≥ mintEnd`, compared in Unix seconds. No mint transaction may have slot `≥ A`.

## 4. Reveal slot and blockhash

1. Target slot `T = A + offsetSlots`.
2. Reveal slot `R` is the smallest produced finalized slot `≥ T`, as returned by `getBlocks(T, …)`.
3. `H` is the base58 `blockhash` of the block at slot `R`, as returned by `getBlock(R)`.

`H` cannot be known when the anchor is fixed (`offsetSlots` ≈ 2 minutes of future blocks), and the operator cannot choose it.

## 5. Starting index and mapping

```
startingIndex = BigInt("0x" + sha256(H + ":" + provenanceHash)) mod N
Founder #k  ↦  art = ((k − 1 + startingIndex) mod N) + 1        for k = 1..S
```

`provenanceHash` is lowercase hex, and `H` is the exact base58 string, joined with a single `:`.

## 6. Final metadata

For every minted asset with mint-time index `k`:

- The asset's on-chain `uri` is `<bundle>/k.json`, where `<bundle>` is the published reveal folder. The on-chain `name` is `Schallern Founder #k`, and so is the JSON `name`.
- The JSON `attributes` equal the attributes of artwork `art` in `collection.json`. The SHA-256 of the image equals the image hash in provenance line `art`.
- The bundle also publishes `provenance.txt`, `collection.json`, `reveal.json` (anchor, `R`, `H`, `startingIndex`, the SHA-256 of this rule file), `_mapping.csv` and `_mints.csv` (`k, asset, signature, slot`). These are for convenience; the verifier recomputes every value from the chain.

## 7. How to verify

Run `node scripts/reveal_verify.mjs --rule <this file or its raw URL> --rule-sha256 <published hash> --bundle <bundle URL>`, with `RPC` set to any mainnet RPC endpoint. The verifier:

1. Prints the SHA-256 of the rule file and compares it with `--rule-sha256`.
2. Checks `provenance.txt` → `provenanceHash` → the hidden settings hash on-chain.
3. Rebuilds the mint set from the chain (section 2) and checks it is exactly `1..S`.
4. Recomputes `A`, `R`, `H` and `startingIndex` independently (sections 3–5) and compares them with `reveal.json`.
5. Checks every asset's `uri`, `name`, attributes and image hash against the mapping, and checks that the collection holds no foreign assets.

Any mismatch is a failure.

## 8. Known limits (stated openly)

- The operator decides *when* to run the reveal, but not *what* it produces: `A`, `R` and `H` follow from the chain alone, and running the reveal again yields the same result.
- The validator that produces slot `R` could withhold that block. `R` would then move to the next produced slot. This one-time skip-or-produce choice is the only influence on `H`, and it lies outside the operator's control.
- If the Candy Guard authority changes the on-chain `endDate` so that it no longer equals `mintEnd`, the not-sold-out reveal fails verification. It does not silently use another anchor.
- Verification needs the full transaction history of the Candy Machine address (archive RPC).
