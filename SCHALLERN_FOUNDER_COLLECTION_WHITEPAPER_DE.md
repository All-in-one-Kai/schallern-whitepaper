# Schallern — Whitepaper Founder Collection

**Version 0.2 · Arbeitsentwurf · 18. Oktober 2026 · Culturetek Pte. Ltd., Singapur**

> Flip the World. Ein Wurf. Eine Wand. Millimeter entscheiden.

## 1. Zusammenfassung

Schallern ist ein physikalisch kalibriertes Münzwurfspiel im Browser: Münze in Richtung Wand werfen; die Münze, deren nächste Kante am nächsten an der Wand liegen bleibt, gewinnt. Das Spiel ist die moderne Fassung eines Schulhofspiels, das in den 80er-Jahren in Deutschland um Milchgeld gespielt wurde. Eine kostenlose, spielbare Demo mit drei Arenen und drei Charakteren ist unter https://schallern.io/play/ live.

Die **Founder Collection** ist eine geplante Serie von **10.000 digitalen Sammlerstücken auf Solana** (Coins und Charaktere). Founder Collectibles sind kosmetisch: Sie verändern, wie Coin und Avatar eines Spielers aussehen, niemals Physik, Geometrie oder Chancen. Der Mint finanziert die nächste Entwicklungsstufe des Spiels. Dieses Whitepaper beschreibt Spiel, Collection, Mint-Mechanik, Mittelverwendung, Roadmap und Team und trennt, was heute live ist, von dem, was geplant ist.

## 2. Das Spiel

**Regel.** Eine Wand, eine Münze je Wurf, drei Runden je Match; die kleinste Summe gewinnt. Gewertet wird der Abstand von der nächsten Münzkante zur Wand in Millimetern, sobald die Münze ruht. Die Münze muss die Wand **nicht** berühren. Eine Münze, die an der Wand lehnt (Lehner), zählt 0 mm. Kamera, Schatten und Optik entscheiden nie über den Sieger; das Physikergebnis entscheidet.

**Fehlwurf und ungültige Würfe.** Der einzige Fehlwurf ist eine Münze, die über die Mauer fliegt. Ungültig ist ein Wurf, wenn der erste Bodenkontakt weniger als 2 m hinter der Abwurflinie liegt (genau auf der 2-m-Linie ist gültig). Fehlwurf und ungültiger Wurf zählen mit der Rundendistanz; kein gültiger Wurf wird schlechter gewertet.

**Rundenkarte.** Vor jeder Runde zeigt eine Karte die Bedingungen, gleich für alle Spieler: die Abwurfdistanz zwischen 6 und 10 m in krummen Werten (zum Beispiel 7,43 m), die Rundenmünze aus einem Katalog echter Münzen in Originalgröße sowie die sichtbaren Boden- und Wandflecken (zum Beispiel Risse, Kies, glatte Stellen oder Blechplatten) und das Gefälle.

**Physik.** Die Münze ist eine dünne Scheibe mit echten Münzdaten, simuliert mit Reibung, Rollwiderstand und Rückprall je Boden (Asphalt, Sand, Marmor) und je Wandmaterial. Das Modell ist physikalisch kalibriert, auf Basis veröffentlichter Messwerte; die Kalibrierung mit gefilmten echten Würfen steht noch aus, deshalb sprechen wir noch nicht von echter Physik. Die Simulation ist deterministisch: gleiche Eingabe, gleiches Ergebnis auf jedem Gerät.

**Steuerung.** Vier Wurfstile: Rutscher (flach und tief), Halbbogen, Hoher Lob und Wandklatscher, jeweils mit eigenem Tempo- und Bogenbereich. Drücken und zurückziehen für Kraft und Richtung, die Geste krümmen für Seitendrall, loslassen, während sich der Abwurf-Ring schließt; Timing und eine ruhige Hand entscheiden über die Güte des Abwurfs. Maus und Touch nutzen dieselbe normierte Eingabe.

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
- **Motive:** Schallern-Coins in acht sichtbaren Trait-Kategorien: Stufe, Material, Finish, Rand, Motiv (darunter die Charaktere des Spiels), Umschrift, Hintergrund (darunter 48 berühmte Wände) und Effekt.
- **Standard:** Metaplex Core auf Solana; jedes Sammlerstück ist ein On-Chain-Asset in einer verifizierten Collection mit On-Chain-Royalty-Information.
- **Seltenheit:** 8 Trait-Kategorien mit 129 Werten; jedes Stück hat jede Kategorie und einen eigenen Seltenheitsrang. Stufen: 11 Einzelstücke (1/1), 89 Legendary, 500 Epic, 1.400 Rare, 3.000 Uncommon und 5.000 Common. Seltenheit ist rein optisches Prestige.
- **Zufällige Zuteilung und Reveal:** Käufer wählen weder Motiv noch Seltenheit noch Stufe. Bis zum Ausverkauf zeigt jedes Sammlerstück denselben Platzhalter. Vor dem Mint wird ein Provenance-Hash der vollständigen, geordneten Collection veröffentlicht und on-chain hinterlegt. Nach dem Ausverkauf ergibt sich der Startversatz aus einem vorab angekündigten künftigen Solana-Slot; so kann niemand, auch nicht das Team, steuern, wer welches Stück bekommt. Jeder kann das Ergebnis gegen den veröffentlichten Hash prüfen.
- **Rechte am Artwork:** Halter dürfen das Artwork ihres Sammlerstücks kommerziell nutzen. Ausgenommen ist die Marke SCHALLERN (Name und Logo); sie bleibt beim Betreiber. Der endgültige Lizenztext wird mit den Mint-Bedingungen veröffentlicht.

## 5. Was ein Founder bekommt, und was nicht

**Bekommt:** das Sammlerstück als Wurf-Skin im Spiel, sobald die Wallet-Verknüpfung live ist; ein Founder-Badge mit der Nummer im Spielerprofil; die Founder-Rolle und Holder-Kanäle auf Discord; eine Stimme bei neuen Arenen und Coin-Designs; frühen Zugang zu neuen Arenen im Spielgeld-Modus; das Recht, das Artwork kommerziell zu nutzen (ohne die Marke SCHALLERN).

**Bekommt nicht:** einen Anteil am Unternehmen, einen Anspruch auf Gewinne, Ausschüttungen, Rückkäufe oder Wertsteigerung, oder irgendeinen Spielvorteil. Die Founder Collection ist ein Sammlerstück, kein Anlageprodukt. Eine Unternehmensfinanzierung ist ein getrenntes, separat strukturiertes Angebot (siehe Abschnitt 10).

## 6. Mint-Mechanik

| Punkt | Plan |
|---|---|
| Chain und Standard | Solana, Metaplex Core, eine Core Candy Machine mit Candy Guard |
| Preisstufen | nach verkaufter Stückzahl, nicht vom Käufer gewählt: #1–4.000 zu 0,5 SOL · #4.001–7.000 zu 1 SOL · #7.001–9.000 zu 1,5 SOL · #9.001–10.000 zu 2 SOL. Wer früh kauft, zahlt weniger; ein Kauf über eine Stufengrenze wird je Stück abgerechnet (geplantes Modell; endgültige Konditionen werden vor dem Start veröffentlicht) |
| Zuteilung | zufälliges Artwork und zufällige Seltenheit für alle 10.000 aus einer Candy Machine, enthüllt nach dem Ausverkauf (siehe Abschnitt 4) |
| Phasen | Start **11. November 2026, 11:11 Uhr SGT (03:11 UTC)**; OG → Allowlist → öffentlich; die Allowlist bedeutet früheren Zugang. Termine und Änderungen nur auf schallern.io und in den offiziellen Discord- und Telegram-Kanälen |
| Grenzen | keine Limits je Wallet, in keiner Phase; Bot-Schutz durch Captcha, Rate-Prüfung und Bot-Tax; jede Mint-Transaktion wird vom Schallern-Backend gebaut und mitsigniert |
| Wo | nur auf schallern.io; das Team schreibt nie zuerst und fragt nie nach Seed-Phrasen |
| Verfügbarkeit | der Mint ist nur dort regional gesperrt, wo es die Bedingungen unserer Dienstleister verlangen |
| Treasury | Mint-Erlöse gehen on-chain in einen 2-von-3-Multisig-Tresor (Squads v4) des Betreibers; kein einzelner Schlüssel kann die Mittel bewegen |
| Royalties | 5 % Sekundär-Royalty, in der Collection hinterlegt |
| Speicher | Artwork und Metadaten auf Arweave (permanent); das endgültige Artwork wird beim Reveal hochgeladen |
| Generalprobe | der komplette Ablauf (Collection, eine Candy Machine mit Platzhalter und On-Chain-Provenance-Hash, Gruppen für Phasen und Preisstufen, Backend-Signer, Geo- und Sanktionsprüfung, Bot- und Lasttests, Reveal aus einem Solana-Slot, öffentliche Prüfung) wurde im Oktober 2026 auf Solana Devnet durchgeführt und geprüft |

Kosten für Käufer: Preis der offenen Stufe plus Solana-Netzwerkgebühren (etwa 0,003 SOL je Mint).

## 7. Mittelverwendung

Die Erlöse finanzieren die nächste Entwicklungsstufe von Schallern. Die geplante Aufteilung umfasst: Spielentwicklung (Multiplayer, Turniere, Accounts), Art und Animation (Produktion der Collection, neue Arenen), Infrastruktur und Sicherheit (Server, RPC, Audits), Community und Marketing (Creator-Programm, Events) sowie eine Betriebsreserve. Die prozentuale Aufteilung und die Szenarien für Mindest-, Ziel- und Ausbaufinanzierung werden vor dem Mint veröffentlicht. Sekundär-Royalties sind nicht Teil des Basisbudgets.

## 8. Roadmap

1. **Jetzt spielbar:** 3D-Demo, drei Arenen, Feinschliff mit Spieler-Feedback, Creator-Programm, Demo-Belohnungen.
2. **Als Nächstes:** die Founder Collection, Community-Aufbau, das finale Mint-Konzept und der Mint.
3. **Geplant:** Online-Matches, Stadt-Crews, Turniere, Spielerkonten mit Rewards- und Affiliate-Dashboards.
4. **Vision:** persönliche physische Figuren, echte Wände, Live-Events.

Abgesehen vom Start des Founder Mint (11. November 2026, 11:11 Uhr SGT) werden Termine nicht versprochen. Jeder Schritt wird angekündigt, wenn er fertig ist.

## 9. Die Spielökonomie (geplanter Echtgeldbetrieb)

Echtgeldspiel ist eine spätere, separat lizenzierte Stufe. Das geplante Modell: Ein Tisch legt den Einsatz fest (zum Beispiel sechs Spieler, drei Runden, 1 USDC je Person); der Sieger erhält den Pot abzüglich einer **Hausgebühr von 10 % auf den positiven Gewinn**; Einsätze und Hausgebühren werden strikt getrennt geführt. Creator, die Spieler bringen, erhalten 36 Monate lang **10 % der bereinigten Hausgebühren** ihrer Spieler (siehe schallern.io/partners.html). Founder Collectibles spielen in dieser Ökonomie keine Rolle, außer dass sie der Skin sind, mit dem ein Spieler wirft.

## 10. Unternehmensfinanzierung (getrennt von der Collection)

Schallern spricht außerdem mit privaten Investoren über eine Finanzierung des Unternehmens (geplantes Mindestinvestment 20.000 EUR). Das ist ein getrenntes, privates Angebot mit eigenen Bedingungen und Unterlagen, nur nach Bewerbung und Prüfung. Es wird nie mit der Founder Collection gebündelt, und nichts in diesem Whitepaper ist Teil davon.

## 11. Team und Betreiber

Betreiber bis zur Gründung der Spielgesellschaft: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Director: Kai Zimmer (Gründer). Team: Kai (Gründer), Pallavi (Finanzen), Riya (Operations), Arsh (Entwicklung), Raj (Entwicklung). Kontakt: mint@schallern.io.

## 12. Technik

- **Spiel:** Three.js Echtzeit-3D, eigene deterministische, physikalisch kalibrierte Coin-Physik, geriggte Charaktere mit Mimik, Telemetrie fürs Balancing. Ergebnisse in Wettbewerbsmodi werden serverseitig berechnet.
- **Mint-Stack:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, Helius RPC, Node-Backend-Signer, Squads-v4-Multisig-Tresor für die Erlöse.
- **Website:** schallern.io (Englisch zuerst, Deutsch), Rechtliches unter schallern.io/legal.html.

## 13. Community und Belohnungen

Discord: https://discord.gg/FpZ5zDjV4. Demo-Tester erhalten Gutscheine für Spielguthaben für qualifiziertes Feedback, für den Discord-Beitritt und für Community-Level (gedeckelt je Person; einlösbar erst beim Echtgeldstart; nicht auszahlbar). Creator verdienen über das Creator-Programm. Regeln: schallern.io/legal.html#rewards und #partners.

## 14. Risiken

Schallern ist in Entwicklung. Die Demo kann sich ändern, die Collection kann sich verzögern, Blockchain-Netzwerke und Wallets können ausfallen, digitale Sammlerstücke können an Wert verlieren, und Echtgeldspiel hängt an Lizenzen, die noch nicht vorliegen. Kaufe nur, was du um seiner selbst willen halten möchtest.

## 15. Rechtlicher Hinweis und Versionen

Rechtsrahmen, Bedingungen, Datenschutz und Disclaimer pflegt die Culturetek Pte. Ltd. und veröffentlicht sie unter https://schallern.io/legal.html. Dieses Dokument ist informativ, kein Angebot zum Verkauf von Wertpapieren und keine Anlageberatung. Versionen dieses Whitepapers werden mit Datum unter schallern.io/whitepaper/ und im dort verlinkten öffentlichen Repository veröffentlicht.

- v0.1 · 16. Oktober 2026 · erster Arbeitsentwurf
- v0.2 · 18. Oktober 2026 · Spielregeln der Demo V04 (keine Wandpflicht, einziger Fehlwurf = über die Mauer, 2-m-Aufsetzlinie, Rundenkarte, vier Wurfstile), Wortlaut „physikalisch kalibriert“, zufällige Zuteilung mit Seltenheiten und Reveal nach Ausverkauf, eine Candy Machine, Preisstufen nach verkaufter Stückzahl, keine Limits je Wallet, Trait-System und Stufenmengen, kommerzielle Nutzung des Artworks, regionale Sperre
