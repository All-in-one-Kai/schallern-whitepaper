# Schallern — Founder Collection Whitepaper

**Version 0.1 · Working draft · 16 October 2026 · Culturetek Pte. Ltd., Singapore**

> Flip the World. One throw. One wall. Millimetres decide.

## 1. Abstract

Schallern is a real-physics coin-throw game played in the browser: throw a coin against a wall, the coin whose edge comes to rest closest to the wall wins. The game is a modern version of a schoolyard game played with milk money in 1980s Germany. A free, playable demo with three arenas and three characters is live at https://schallern.io/play/.

The **Founder Collection** is a planned series of **10,000 digital collectibles on Solana** (coins and characters). Founder Collectibles are cosmetic: they change how a player's coin and avatar look, they never change physics, geometry or odds. The mint finances the next development stage of the game. This whitepaper describes the game, the collection, the mint mechanics, the use of proceeds, the roadmap and the team, and separates what is live today from what is planned.

## 2. The game

**Rule.** One wall, one coin per throw, three rounds per match. After three rounds the smallest sum of distances wins. A throw that never touches the wall, leaves the lane, flies over the wall or rebounds more than 150 cm is a foul and counts the published maximum distance.

**Measurement.** The distance is measured from the nearest edge of the coin to the wall after the coin has come to rest, quantised to a published millimetre grid. The camera, shadows and visuals never decide a winner; the physics result does.

**Physics.** The coin is a rigid thin disc simulated at a fixed 240 Hz step with velocity-dependent restitution, rolling friction per surface (asphalt, sand, marble) and wall materials (concrete, sandstone, lacquer). Every player in a round throws under the same distance, surface and wall. Throws are deterministic for the same input.

**Controls.** Drag down for power, drag sideways for direction, a slider for the arc; mouse and touch share the same normalised input limits. The release is shown in slow motion with a five-finger hand and thumb flick.

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
- **Subjects:** Schallern coins (materials, finishes, edges, engravings, patina) and characters in the style of the game's own figures; optional arena themes from a catalogue of 48 famous walls.
- **Standard:** Metaplex Core on Solana; each collectible is one on-chain asset in a verified collection with on-chain royalty information.
- **Rarity:** a trait system (about 8 to 12 trait categories, 200 to 300 variants) gives every piece its own rarity rank from 1 to 10,000, plus five marketing tiers and a small number of 1/1 specials. Rarity is prestige only.
- **Reveal:** whether buyers choose their tier without a random reveal, or artwork is revealed on a reveal day, is an open product decision; it is published before the mint opens.
- **Artwork rights:** holders receive a personal, non-exclusive licence to their artwork; the SCHALLERN word mark stays with the operator. The final licence text is published with the mint terms.

## 5. What a founder gets, and what a founder does not get

**Gets:** the collectible as a throwing skin in the game once wallet linking is live; a Founder badge with the collectible number on the player profile; the Founder role and holder channels on Discord; a vote on which arenas and coin designs come next; early access to new arenas in play-money mode.

**Does not get:** a stake in the company, a claim to profits, distributions, buy-backs or value increase, or any gameplay advantage. The Founder Collection is a collectible, not an investment product. Any company financing is a separate, separately structured offer (see section 10).

## 6. Mint mechanics

| Item | Plan |
|---|---|
| Chain and standard | Solana, Metaplex Core, Core Candy Machine with Candy Guard |
| Tiers and prices | #1–4,000 at 0.5 SOL · #4,001–7,000 at 1 SOL · #7,001–9,000 at 1.5 SOL · #9,001–10,000 at 2 SOL (planned model; final terms are published before the start) |
| Phases | team and OG → allowlist (guaranteed, limited per wallet) → waitlist raffle → public; dates are announced on schallern.io and in the Discord announcements channel only |
| Limits | per-wallet mint limits per phase; bot tax; every mint transaction is built and co-signed by the Schallern backend after captcha and rate checks |
| Where | only on schallern.io; the team never messages first and never asks for seed phrases |
| Treasury | mint proceeds go directly to a multi-signature treasury (2-of-3) |
| Royalties | 5 % secondary royalty, written into the collection |
| Storage | artwork and metadata on Arweave (permanent) |
| Rehearsal | the complete flow (collection, four tier machines with phase groups, allowlist proofs, backend signer, bot and load tests, Arweave upload, reveal update) has been run and verified on Solana devnet in October 2026 |

Mint costs for buyers are the tier price plus Solana network fees (about 0.003 SOL per mint).

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

- **Game:** Three.js real-time 3D, custom deterministic coin physics, rigged characters with facial animation, telemetry for balancing. Results in competitive modes will be computed server-side.
- **Mint stack:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave via Irys, Helius RPC, a Node backend signer, Squads multisig.
- **Website:** schallern.io (English first, German), legal pages at schallern.io/legal.html.

## 13. Community and rewards

Discord: https://discord.gg/FpZ5zDjV4. Demo testers earn play-credit vouchers for qualified feedback, for joining Discord and for community levels (capped per person; redeemable only at the real-money launch; not cashable). Creators earn through the creator programme. Rules: schallern.io/legal.html#rewards and #partners.

## 14. Risks

Schallern is in development. The demo may change, the collection may be delayed, blockchain networks and wallets can fail, digital collectibles can lose value, and real-money play depends on licences that are not yet in place. Buy only what you can afford to hold for its own sake.

## 15. Legal notice and versions

The legal framework, terms, privacy and disclaimers are maintained by Culturetek Pte. Ltd. and published at https://schallern.io/legal.html. This document is informational, not an offer to sell securities and not investment advice. Versions of this whitepaper are published with their date at schallern.io/whitepaper/ and in the public repository linked there.

- v0.1 · 16 October 2026 · first working draft
