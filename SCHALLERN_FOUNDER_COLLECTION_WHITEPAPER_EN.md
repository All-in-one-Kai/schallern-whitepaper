# Schallern — Founder Collection Whitepaper

**Version 0.2 · Working draft · 18 October 2026 · Culturetek Pte. Ltd., Singapore**

> Flip the World. One throw. One wall. Millimetres decide.

## 1. Abstract

Schallern is a physically calibrated coin-throw game played in the browser: throw a coin towards a wall; the coin whose nearest edge comes to rest closest to the wall wins. The game is a modern version of a schoolyard game played with milk money in 1980s Germany. A free, playable demo with three arenas and three characters is live at https://schallern.io/play/.

The **Founder Collection** is a planned series of **10,000 digital collectibles on Solana** (coins and characters). Founder Collectibles are cosmetic: they change how a player's coin and avatar look, they never change physics, geometry or odds. The mint finances the next development stage of the game. This whitepaper describes the game, the collection, the mint mechanics, the use of proceeds, the roadmap and the team, and separates what is live today from what is planned.

## 2. The game

**Rule.** One wall, one coin per throw, three rounds per match; the smallest total wins. A throw scores the distance from the nearest edge of the coin to the wall, in millimetres, once the coin has come to rest. The coin does **not** have to touch the wall. A coin left leaning against the wall (a leaner) scores 0 mm. The camera, shadows and visuals never decide a winner; the physics result does.

**Foul and invalid throws.** The only foul is a coin that flies over the wall. A throw is invalid if the coin's first ground contact is less than 2 m past the throw line (landing exactly on the 2 m line is valid). A foul or an invalid throw counts the round distance; no valid throw can score worse than that.

**Round card.** Before every round a card shows the conditions, the same for every player: the throwing distance between 6 and 10 m in odd values (for example 7.43 m), the round coin from a catalogue of real coins in their real sizes, and the visible ground and wall patches (for example cracks, gravel, smooth spots or metal plates) and the slope.

**Physics.** The coin is a thin disc with real coin data, simulated with friction, rolling resistance and bounce per surface (asphalt, sand, marble) and per wall material. The model is physically calibrated from published measurements; a calibration against filmed real throws is still pending, so we do not call it real physics yet. The simulation is deterministic: the same input gives the same result on every device.

**Controls.** Four throw styles: Slider (low and flat), Half-arc, High lob and Wall slap, each with its own speed and arc range. Press and pull back for power and direction, curve the gesture for side spin, and release while the shrinking release ring closes; timing and a steady hand decide the quality of the release. Mouse and touch use the same normalised input.

**Fairness.** Nothing a player can buy changes mass, diameter, friction, bounce or precision. Rarity is visual. This is the founding rule of the project and applies to every collectible described here.

## 3. Status today (what is live, what is not)

| Live today | Not yet |
|---|---|
| Free browser demo at schallern.io/play/, desktop and mobile, no wallet | Real-money tables (only after licensing, audit and approval, and only in permitted countries) |
| Three arenas (Berlin asphalt, Giza sand, Vegas marble), three characters (NEO, MAYA, BO), local AI opponents | Online multiplayer, tournaments, city crews |
| Feedback chat with rewards, creator programme with tracking links, newsletter | Founder Mint on mainnet (the full flow has been rehearsed on Solana devnet, see section 6) |
| Discord server with the Schallern Rewards bot | Wallet linking in the game |

Demo points have no cash value. No NFT, token or payment is created by playing the demo.

## 4. The Founder Collection

- **Supply:** 10,000 collectibles, numbered.
- **Subjects:** Schallern coins in eight visible trait categories: tier, material, finish, edge, motif (including the game's characters), inscription, backdrop (including 48 famous walls) and effect.
- **Standard:** Metaplex Core on Solana; each collectible is one on-chain asset in a verified collection with on-chain royalty information.
- **Rarity:** 8 trait categories with 129 values; every piece has every category and its own rarity rank. Tiers: 11 one-of-one pieces (1/1), 89 Legendary, 500 Epic, 1,400 Rare, 3,000 Uncommon and 5,000 Common. Rarity is visual prestige only.
- **Random assignment and reveal:** buyers do not choose artwork, rarity or tier. Until sell-out every collectible shows the same placeholder. Before the mint opens, a provenance hash of the complete, ordered collection is published and stored on-chain. After sell-out the starting offset is taken from a pre-announced future Solana slot, so nobody, not even the team, can steer who gets which piece. Anyone can check the result against the published hash.
- **Artwork rights:** holders may use the artwork of their collectible commercially. The SCHALLERN brand (name and logo) is excluded and stays with the operator. The final licence text is published with the mint terms.

## 5. What a founder gets, and what a founder does not get

**Gets:** the collectible as a throwing skin in the game once wallet linking is live; a Founder badge with the collectible number on the player profile; the Founder role and holder channels on Discord; a vote on which arenas and coin designs come next; early access to new arenas in play-money mode; the right to use the artwork commercially (SCHALLERN brand excluded).

**Does not get:** a stake in the company, a claim to profits, distributions, buy-backs or value increase, or any gameplay advantage. The Founder Collection is a collectible, not an investment product. Any company financing is a separate, separately structured offer (see section 10).

## 6. Mint mechanics

| Item | Plan |
|---|---|
| Chain and standard | Solana, Metaplex Core, one Core Candy Machine with Candy Guard |
| Price steps | set by the number sold, not chosen by the buyer: #1–4,000 at 0.5 SOL · #4,001–7,000 at 1 SOL · #7,001–9,000 at 1.5 SOL · #9,001–10,000 at 2 SOL. Early buyers pay less; a purchase that crosses a step is priced per piece (planned model; final terms are published before the start) |
| Assignment | random artwork and rarity for all 10,000 from one Candy Machine, revealed after sell-out (see section 4) |
| Phases | OG → allowlist → public; the allowlist means earlier access. Dates are announced only on schallern.io and in the official Discord and Telegram channels |
| Limits | no per-wallet limits in any phase; bot protection through captcha, rate checks and bot tax; every mint transaction is built and co-signed by the Schallern backend |
| Where | only on schallern.io; the team never messages first and never asks for seed phrases |
| Availability | the mint is geo-restricted only where the terms of our service providers require it |
| Treasury | mint proceeds are paid on-chain directly to the operator's treasury wallet |
| Royalties | 5 % secondary royalty, written into the collection |
| Storage | artwork and metadata on Arweave (permanent); final artwork is uploaded at the reveal |
| Rehearsal | the complete flow (collection, one Candy Machine with placeholder and on-chain provenance hash, phase and price-step groups, backend signer, geo and sanctions checks, bot and load tests, reveal from a Solana slot, public verification) has been run and verified on Solana devnet in October 2026 |

Mint costs for buyers are the price of the open step plus Solana network fees (about 0.003 SOL per mint).

## 7. Use of proceeds

Proceeds finance the next development stage of Schallern. The planned allocation covers: game development (multiplayer, tournaments, accounts), art and animation (collection production, new arenas), infrastructure and security (servers, RPC, audits), community and marketing (creator programme, events) and an operating reserve. The percentage split and the minimum, target and extended funding scenarios are published before the mint opens. Secondary royalties are not part of the base budget.

## 8. Roadmap

1. **Playable now:** 3D demo, three arenas, fine-tuning with player feedback, creator programme, demo rewards.
2. **Next:** the Founder Collection, community growth, the final mint concept and the mint.
3. **Planned:** online matches, city crews, tournaments, player accounts with rewards and affiliate dashboards.
4. **Vision:** personal physical figures, real walls, live events.

Dates are not promised. Every step is announced when it is ready.

## 9. The game economy (planned real-money mode)

Real-money play is a later, separately licensed stage. The planned model: a table sets the stake (for example six players, three rounds, 1 USDC each); the winner takes the pot minus a **10 % house fee on the positive win**; stakes and house fees are kept strictly apart. Creators who bring players receive **10 % of the adjusted house fees** of their players for 36 months (see schallern.io/partners.html). Founder Collectibles play no role in this economy other than being the skin a player throws with.

## 10. Company financing (separate from the collection)

Schallern also talks to private investors about financing the company (planned minimum EUR 20,000). That is a separate, private offer with its own terms and documents, available only after application and review. It is never bundled with the Founder Collection, and nothing in this whitepaper is part of it.

## 11. Team and operator

Operator until the game company is founded: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Director: Kai Zimmer (founder). Team: Kai (founder), Pallavi (finance), Riya (operations), Arsh (development), Raj (development). Contact: mint@schallern.io.

## 12. Technology

- **Game:** Three.js real-time 3D, custom deterministic and physically calibrated coin physics, rigged characters with facial animation, telemetry for balancing. Results in competitive modes will be computed server-side.
- **Mint stack:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, Helius RPC, a Node backend signer.
- **Website:** schallern.io (English first, German), legal pages at schallern.io/legal.html.

## 13. Community and rewards

Discord: https://discord.gg/FpZ5zDjV4. Demo testers earn play-credit vouchers for qualified feedback, for joining Discord and for community levels (capped per person; redeemable only at the real-money launch; not cashable). Creators earn through the creator programme. Rules: schallern.io/legal.html#rewards and #partners.

## 14. Risks

Schallern is in development. The demo may change, the collection may be delayed, blockchain networks and wallets can fail, digital collectibles can lose value, and real-money play depends on licences that are not yet in place. Buy only what you can afford to hold for its own sake.

## 15. Legal notice and versions

The legal framework, terms, privacy and disclaimers are maintained by Culturetek Pte. Ltd. and published at https://schallern.io/legal.html. This document is informational, not an offer to sell securities and not investment advice. Versions of this whitepaper are published with their date at schallern.io/whitepaper/ and in the public repository linked there.

- v0.1 · 16 October 2026 · first working draft
- v0.2 · 18 October 2026 · game rules of demo V04 (no wall touch required, only foul = over the wall, 2 m touchdown line, round card, four throw styles), "physically calibrated" wording, random assignment with rarities and reveal after sell-out, one Candy Machine, price steps by number sold, no per-wallet limits, trait system and tier counts, commercial use of artwork, geo restriction
