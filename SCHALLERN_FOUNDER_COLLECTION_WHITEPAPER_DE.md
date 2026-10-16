# Schallern — Whitepaper Founder Collection

**Version 0.1 · Arbeitsentwurf · 16. Oktober 2026 · Culturetek Pte. Ltd., Singapur**

> Flip the World. Ein Wurf. Eine Wand. Millimeter entscheiden.

## 1. Zusammenfassung

Schallern ist ein Münzwurfspiel mit echter Physik im Browser: Münze gegen die Wand werfen, die Münze, deren Kante am nächsten an der Wand liegen bleibt, gewinnt. Das Spiel ist die moderne Fassung eines Schulhofspiels, das in den 80er-Jahren in Deutschland um Milchgeld gespielt wurde. Eine kostenlose, spielbare Demo mit drei Arenen und drei Charakteren ist unter https://schallern.io/play/ live.

Die **Founder Collection** ist eine geplante Serie von **10.000 digitalen Sammlerstücken auf Solana** (Coins und Charaktere). Founder Collectibles sind kosmetisch: Sie verändern, wie Coin und Avatar eines Spielers aussehen, niemals Physik, Geometrie oder Chancen. Der Mint finanziert die nächste Entwicklungsstufe des Spiels. Dieses Whitepaper beschreibt Spiel, Collection, Mint-Mechanik, Mittelverwendung, Roadmap und Team und trennt, was heute live ist, von dem, was geplant ist.

## 2. Das Spiel

**Regel.** Eine Wand, eine Münze je Wurf, drei Runden je Match. Nach drei Runden gewinnt die kleinste Summe der Abstände. Ein Wurf, der die Wand nie berührt, die Bahn verlässt, über die Wand fliegt oder mehr als 150 cm zurückprallt, ist ein Fehlwurf und zählt mit der veröffentlichten Maximaldistanz.

**Messung.** Gemessen wird vom nächsten Münzrand zur Wand nach dem Stillstand, quantisiert auf ein veröffentlichtes Millimeterraster. Kamera, Schatten und Optik entscheiden nie über den Sieger; das Physikergebnis entscheidet.

**Physik.** Die Münze ist eine starre, dünne Scheibe, simuliert mit festem 240-Hz-Schritt, geschwindigkeitsabhängigem Rückprall, Rollreibung je Boden (Asphalt, Sand, Marmor) und Wandmaterialien (Beton, Sandstein, Lack). Alle Spieler einer Runde werfen unter derselben Distanz, demselben Boden und derselben Wand. Gleiche Eingabe, gleiches Ergebnis.

**Steuerung.** Nach unten ziehen für Kraft, seitlich für Richtung, ein Regler für den Bogen; Maus und Touch teilen dieselben normierten Eingabegrenzen. Der Abwurf wird in Zeitlupe mit fünf Fingern und Daumen-Flip gezeigt.

**Fairness.** Nichts, was ein Spieler kaufen kann, verändert Masse, Durchmesser, Reibung, Rückprall oder Präzision. Seltenheit ist optisch. Das ist die Gründungsregel des Projekts und gilt für jedes hier beschriebene Sammlerstück.

## 3. Stand heute (was live ist, was nicht)

| Live heute | Noch nicht |
|---|---|
| Kostenlose Browser-Demo unter schallern.io/play/, Desktop und Handy, ohne Wallet | Echtgeld-Tische (erst nach Lizenz, Audit und Freigabe, nur in erlaubten Ländern) |
| Drei Arenen (Berlin Asphalt, Giza Sand, Vegas Marmor), drei Charaktere (NEO, MAYA, BO), lokale KI-Gegner | Online-Multiplayer, Turniere, Stadt-Crews |
| Feedback-Chat mit Belohnungen, Creator-Programm mit Tracking-Links, Newsletter | Founder Mint auf Mainnet (der komplette Ablauf wurde auf Solana Devnet geprobt, siehe Abschnitt 6) |
| Discord-Server mit dem Bot „Schallern Rewards“ | Wallet-Verknüpfung im Spiel |

Demo-Punkte haben keinen Geldwert. Durch das Spielen der Demo entsteht kein NFT, kein Token und keine Zahlung.

## 4. Die Founder Collection

- **Auflage:** 10.000 Sammlerstücke, nummeriert.
- **Motive:** Schallern-Coins (Materialien, Finishs, Kanten, Gravuren, Patina) und Charaktere im Stil der Spielfiguren; optional Arena-Themen aus einem Katalog von 48 berühmten Wänden.
- **Standard:** Metaplex Core auf Solana; jedes Sammlerstück ist ein On-Chain-Asset in einer verifizierten Collection mit On-Chain-Royalty-Information.
- **Seltenheit:** ein Trait-System (etwa 8 bis 12 Kategorien, 200 bis 300 Varianten) gibt jedem Stück einen eigenen Seltenheitsrang von 1 bis 10.000, dazu fünf Marketing-Stufen und wenige 1/1-Specials. Seltenheit ist reines Prestige.
- **Reveal:** ob Käufer ihre Stufe ohne Zufalls-Reveal wählen oder das Artwork an einem Reveal-Tag enthüllt wird, ist eine offene Produktentscheidung; sie wird vor dem Mint veröffentlicht.
- **Rechte am Artwork:** Halter erhalten eine persönliche, nicht ausschließliche Lizenz an ihrem Artwork; die Wortmarke SCHALLERN bleibt beim Betreiber. Der endgültige Lizenztext wird mit den Mint-Bedingungen veröffentlicht.

## 5. Was ein Founder bekommt, und was nicht

**Bekommt:** das Sammlerstück als Wurf-Skin im Spiel, sobald die Wallet-Verknüpfung live ist; ein Founder-Badge mit der Nummer im Spielerprofil; die Founder-Rolle und Holder-Kanäle auf Discord; eine Stimme bei neuen Arenen und Coin-Designs; frühen Zugang zu neuen Arenen im Spielgeld-Modus.

**Bekommt nicht:** einen Anteil am Unternehmen, einen Anspruch auf Gewinne, Ausschüttungen, Rückkäufe oder Wertsteigerung, oder irgendeinen Spielvorteil. Die Founder Collection ist ein Sammlerstück, kein Anlageprodukt. Eine Unternehmensfinanzierung ist ein getrenntes, separat strukturiertes Angebot (siehe Abschnitt 10).

## 6. Mint-Mechanik

| Punkt | Plan |
|---|---|
| Chain und Standard | Solana, Metaplex Core, Core Candy Machine mit Candy Guard |
| Stufen und Preise | #1–4.000 zu 0,5 SOL · #4.001–7.000 zu 1 SOL · #7.001–9.000 zu 1,5 SOL · #9.001–10.000 zu 2 SOL (geplantes Modell; endgültige Konditionen werden vor dem Start veröffentlicht) |
| Phasen | Team und OG → Allowlist (garantiert, begrenzt je Wallet) → Warteliste per Verlosung → öffentlich; Termine nur auf schallern.io und im Discord-Ankündigungskanal |
| Grenzen | Mint-Limits je Wallet und Phase; Bot-Tax; jede Mint-Transaktion wird vom Schallern-Backend nach Captcha- und Rate-Prüfung gebaut und mitsigniert |
| Wo | nur auf schallern.io; das Team schreibt nie zuerst und fragt nie nach Seed-Phrasen |
| Treasury | Mint-Erlöse gehen direkt in eine Multi-Signatur-Treasury (2 von 3) |
| Royalties | 5 % Sekundär-Royalty, in der Collection hinterlegt |
| Speicher | Artwork und Metadaten auf Arweave (permanent) |
| Generalprobe | der komplette Ablauf (Collection, vier Stufen-Maschinen mit Phasengruppen, Allowlist-Nachweise, Backend-Signer, Bot- und Lasttests, Arweave-Upload, Reveal-Update) wurde im Oktober 2026 auf Solana Devnet durchgeführt und geprüft |

Kosten für Käufer: Stufenpreis plus Solana-Netzwerkgebühren (etwa 0,003 SOL je Mint).

## 7. Mittelverwendung

Die Erlöse finanzieren die nächste Entwicklungsstufe von Schallern. Die geplante Aufteilung umfasst: Spielentwicklung (Multiplayer, Turniere, Accounts), Art und Animation (Produktion der Collection, neue Arenen), Infrastruktur und Sicherheit (Server, RPC, Audits), Community und Marketing (Creator-Programm, Events) sowie eine Betriebsreserve. Die prozentuale Aufteilung und die Szenarien für Mindest-, Ziel- und Ausbaufinanzierung werden vor dem Mint veröffentlicht. Sekundär-Royalties sind nicht Teil des Basisbudgets.

## 8. Roadmap

1. **Jetzt spielbar:** 3D-Demo, drei Arenen, Feinschliff mit Spieler-Feedback, Creator-Programm, Demo-Belohnungen.
2. **Als Nächstes:** die Founder Collection, Community-Aufbau, das finale Mint-Konzept und der Mint.
3. **Geplant:** Online-Matches, Stadt-Crews, Turniere, Spielerkonten mit Rewards- und Affiliate-Dashboards.
4. **Vision:** persönliche physische Figuren, echte Wände, Live-Events.

Termine werden nicht versprochen. Jeder Schritt wird angekündigt, wenn er fertig ist.

## 9. Die Spielökonomie (geplanter Echtgeldbetrieb)

Echtgeldspiel ist eine spätere, separat lizenzierte Stufe. Das geplante Modell: Ein Tisch legt den Einsatz fest (zum Beispiel sechs Spieler, drei Runden, 1 USDC je Person); der Sieger erhält den Pot abzüglich einer **Hausgebühr von 10 % auf den positiven Gewinn**; Einsätze und Hausgebühren werden strikt getrennt geführt. Creator, die Spieler bringen, erhalten 36 Monate lang **10 % der bereinigten Hausgebühren** ihrer Spieler (siehe schallern.io/partners.html). Founder Collectibles spielen in dieser Ökonomie keine Rolle, außer dass sie der Skin sind, mit dem ein Spieler wirft.

## 10. Unternehmensfinanzierung (getrennt von der Collection)

Schallern spricht außerdem mit privaten Investoren über eine Finanzierung des Unternehmens (geplantes Mindestinvestment 20.000 EUR). Das ist ein getrenntes, privates Angebot mit eigenen Bedingungen und Unterlagen, nur nach Bewerbung und Prüfung. Es wird nie mit der Founder Collection gebündelt, und nichts in diesem Whitepaper ist Teil davon.

## 11. Team und Betreiber

Betreiber bis zur Gründung der Spielgesellschaft: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Director: Kai Zimmer (Gründer). Team: Kai (Gründer), Pallavi (Finanzen), Riya (Operations), Arsh (Entwicklung), Raj (Entwicklung). Kontakt: mint@schallern.io.

## 12. Technik

- **Spiel:** Three.js Echtzeit-3D, eigene deterministische Coin-Physik, geriggte Charaktere mit Mimik, Telemetrie fürs Balancing. Ergebnisse in Wettbewerbsmodi werden serverseitig berechnet.
- **Mint-Stack:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave über Irys, Helius RPC, Node-Backend-Signer, Squads-Multisig.
- **Website:** schallern.io (Englisch zuerst, Deutsch), Rechtliches unter schallern.io/legal.html.

## 13. Community und Belohnungen

Discord: https://discord.gg/FpZ5zDjV4. Demo-Tester erhalten Gutscheine für Spielguthaben für qualifiziertes Feedback, für den Discord-Beitritt und für Community-Level (gedeckelt je Person; einlösbar erst beim Echtgeldstart; nicht auszahlbar). Creator verdienen über das Creator-Programm. Regeln: schallern.io/legal.html#rewards und #partners.

## 14. Risiken

Schallern ist in Entwicklung. Die Demo kann sich ändern, die Collection kann sich verzögern, Blockchain-Netzwerke und Wallets können ausfallen, digitale Sammlerstücke können an Wert verlieren, und Echtgeldspiel hängt an Lizenzen, die noch nicht vorliegen. Kaufe nur, was du um seiner selbst willen halten möchtest.

## 15. Rechtlicher Hinweis und Versionen

Rechtsrahmen, Bedingungen, Datenschutz und Disclaimer pflegt die Culturetek Pte. Ltd. und veröffentlicht sie unter https://schallern.io/legal.html. Dieses Dokument ist informativ, kein Angebot zum Verkauf von Wertpapieren und keine Anlageberatung. Versionen dieses Whitepapers werden mit Datum unter schallern.io/whitepaper/ und im dort verlinkten öffentlichen Repository veröffentlicht.

- v0.1 · 16. Oktober 2026 · erster Arbeitsentwurf
