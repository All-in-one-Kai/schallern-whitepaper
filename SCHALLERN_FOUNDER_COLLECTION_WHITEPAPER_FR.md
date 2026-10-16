# Schallern — Whitepaper Founder Collection

**Version 0.1 · Projet de travail · 16 octobre 2026 · Culturetek Pte. Ltd., Singapour**

> Flip the World. Un lancer. Un mur. Les millimètres décident.

## 1. Résumé

Schallern est un jeu de lancer de pièces à physique réelle, joué dans le navigateur : lance une pièce contre un mur, la pièce dont le bord s’immobilise le plus près du mur gagne. Le jeu est une version moderne d’un jeu de cour de récré joué avec l’argent du lait dans l’Allemagne des années 1980. Une démo gratuite et jouable avec trois arènes et trois personnages est en ligne sur https://schallern.io/play/.

La **Founder Collection** est une série prévue de **10 000 objets de collection numériques sur Solana** (pièces et personnages). Les Founder Collectibles sont cosmétiques : ils changent l’apparence de la pièce et de l’avatar d’un joueur, jamais la physique, la géométrie ou les chances. Le mint finance la prochaine étape de développement du jeu. Ce whitepaper décrit le jeu, la collection, la mécanique du mint, l’emploi des fonds, la roadmap et l’équipe, et distingue ce qui est en ligne aujourd’hui de ce qui est prévu.

## 2. Le jeu

**Règle.** Un mur, une pièce par lancer, trois manches par match. Après trois manches, la plus petite somme des distances gagne. Un lancer qui ne touche jamais le mur, sort du couloir, passe par-dessus le mur ou rebondit de plus de 150 cm est une faute et compte pour la distance maximale publiée.

**Mesure.** La distance est mesurée du bord de la pièce le plus proche jusqu’au mur une fois la pièce immobilisée, quantifiée sur une grille millimétrique publiée. La caméra, les ombres et les visuels ne décident jamais d’un vainqueur ; le résultat physique le fait.

**Physique.** La pièce est un disque mince rigide simulé à un pas fixe de 240 Hz avec une restitution dépendante de la vitesse, une friction de roulement par surface (asphalte, sable, marbre) et des matériaux de mur (béton, grès, laque). Chaque joueur d’une manche lance avec la même distance, la même surface et le même mur. Les lancers sont déterministes pour une même entrée.

**Commandes.** Glisse vers le bas pour la puissance, latéralement pour la direction, un curseur pour la courbe ; souris et tactile partagent les mêmes limites d’entrée normalisées. Le lâcher est montré au ralenti avec une main à cinq doigts et une pichenette du pouce.

**Équité.** Rien de ce qu’un joueur peut acheter ne change la masse, le diamètre, la friction, le rebond ou la précision. La rareté est visuelle. C’est la règle fondatrice du projet et elle s’applique à chaque objet de collection décrit ici.

## 3. État actuel (ce qui est en ligne, ce qui ne l’est pas)

| En ligne aujourd’hui | Pas encore |
|---|---|
| Démo gratuite dans le navigateur sur schallern.io/play/, desktop et mobile, sans wallet | Tables en argent réel (uniquement après licence, audit et validation, et uniquement dans les pays autorisés) |
| Trois arènes (asphalte de Berlin, sable de Giza, marbre de Vegas), trois personnages (NEO, MAYA, BO), adversaires IA locaux | Multijoueur en ligne, tournois, crews de ville |
| Chat de feedback avec récompenses, Programme créateurs avec liens de suivi, newsletter | Founder Mint sur le mainnet (le flux complet a été répété sur le devnet Solana, voir section 6) |
| Serveur Discord avec le bot Schallern Rewards | Liaison du wallet dans le jeu |

Les points de la démo n’ont aucune valeur monétaire. Aucun NFT, token ou paiement n’est créé en jouant à la démo.

## 4. La Founder Collection

- **Offre :** 10 000 objets de collection, numérotés.
- **Sujets :** pièces Schallern (matériaux, finitions, tranches, gravures, patine) et personnages dans le style des figures du jeu ; thèmes d’arènes optionnels issus d’un catalogue de 48 murs célèbres.
- **Standard :** Metaplex Core sur Solana ; chaque objet de collection est un asset on-chain dans une collection vérifiée avec des informations de royalties on-chain.
- **Rareté :** un système de traits (environ 8 à 12 catégories de traits, 200 à 300 variantes) donne à chaque pièce son propre rang de rareté de 1 à 10 000, plus cinq paliers marketing et un petit nombre de pièces spéciales 1/1. La rareté n’est que du prestige.
- **Reveal :** savoir si les acheteurs choisissent leur palier sans reveal aléatoire, ou si l’artwork est révélé un jour de reveal, est une décision produit ouverte ; elle est publiée avant l’ouverture du mint.
- **Droits sur l’artwork :** les holders reçoivent une licence personnelle et non exclusive sur leur artwork ; la marque verbale SCHALLERN reste à l’opérateur. Le texte final de la licence est publié avec les conditions du mint.

## 5. Ce qu’un Founder reçoit, et ce qu’un Founder ne reçoit pas

**Reçoit :** l’objet de collection comme skin de lancer dans le jeu dès que la liaison du wallet est active ; un badge Founder avec le numéro de l’objet sur le profil de joueur ; le rôle Founder et les salons réservés aux holders sur Discord ; un vote sur les prochaines arènes et les prochains designs de pièces ; un accès anticipé aux nouvelles arènes en mode argent fictif.

**Ne reçoit pas :** une participation dans la société, un droit à des bénéfices, distributions, rachats ou plus-values, ni aucun avantage de gameplay. La Founder Collection est un objet de collection, pas un produit d’investissement. Tout financement de la société est une offre distincte, structurée séparément (voir section 10).

## 6. Mécanique du mint

| Élément | Plan |
|---|---|
| Chaîne et standard | Solana, Metaplex Core, Core Candy Machine avec Candy Guard |
| Paliers et prix | #1–4 000 à 0,5 SOL · #4 001–7 000 à 1 SOL · #7 001–9 000 à 1,5 SOL · #9 001–10 000 à 2 SOL (modèle prévu ; les conditions définitives sont publiées avant le lancement) |
| Phases | équipe et OG → Allowlist (garantie, limitée par wallet) → tirage au sort de la liste d’attente → public ; les dates sont annoncées uniquement sur schallern.io et dans le salon d’annonces du Discord |
| Limites | limites de mint par wallet et par phase ; taxe anti-bot ; chaque transaction de mint est construite et cosignée par le backend Schallern après captcha et contrôles de fréquence |
| Où | uniquement sur schallern.io ; l’équipe n’écrit jamais en premier et ne demande jamais de seed phrase |
| Trésorerie | les produits du mint vont directement dans une trésorerie multi-signature (2 sur 3) |
| Royalties | 5 % de royalties sur le marché secondaire, inscrites dans la collection |
| Stockage | artwork et métadonnées sur Arweave (permanent) |
| Répétition | le flux complet (collection, quatre machines de palier avec groupes de phases, preuves d’Allowlist, signataire backend, tests anti-bot et de charge, upload Arweave, mise à jour du reveal) a été exécuté et vérifié sur le devnet Solana en octobre 2026 |

Les coûts de mint pour les acheteurs sont le prix du palier plus les frais de réseau Solana (environ 0,003 SOL par mint).

## 7. Emploi des fonds

Les produits financent la prochaine étape de développement de Schallern. L’allocation prévue couvre : le développement du jeu (multijoueur, tournois, comptes), l’art et l’animation (production de la collection, nouvelles arènes), l’infrastructure et la sécurité (serveurs, RPC, audits), la communauté et le marketing (Programme créateurs, événements) et une réserve d’exploitation. La répartition en pourcentage ainsi que les scénarios de financement minimum, cible et étendu sont publiés avant l’ouverture du mint. Les royalties secondaires ne font pas partie du budget de base.

## 8. Roadmap

1. **Jouable maintenant :** démo 3D, trois arènes, réglages fins avec les retours des joueurs, Programme créateurs, récompenses démo.
2. **Ensuite :** la Founder Collection, la croissance de la communauté, le concept final du mint et le mint.
3. **Prévu :** matchs en ligne, crews de ville, tournois, comptes joueurs avec récompenses et tableaux de bord d’affiliation.
4. **Vision :** figurines physiques personnelles, vrais murs, événements live.

Les dates ne sont pas promises. Chaque étape est annoncée quand elle est prête.

## 9. L’économie du jeu (mode argent réel prévu)

Le jeu en argent réel est une étape ultérieure, licenciée séparément. Le modèle prévu : une table fixe la mise (par exemple six joueurs, trois manches, 1 USDC chacun) ; le vainqueur remporte le pot moins une **commission de la maison de 10 % sur le gain positif** ; les mises et les commissions de la maison sont strictement séparées. Les créateurs qui amènent des joueurs reçoivent **10 % des commissions de la maison ajustées** de leurs joueurs pendant 36 mois (voir schallern.io/partners.html). Les Founder Collectibles ne jouent aucun rôle dans cette économie, si ce n’est d’être le skin avec lequel un joueur lance.

## 10. Financement de la société (distinct de la collection)

Schallern discute également avec des investisseurs privés du financement de la société (minimum prévu : 20 000 EUR). Il s’agit d’une offre distincte et privée avec ses propres conditions et documents, accessible uniquement après candidature et examen. Elle n’est jamais couplée à la Founder Collection, et rien dans ce whitepaper n’en fait partie.

## 11. Équipe et opérateur

Opérateur jusqu’à la création de la société du jeu : **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Directeur : Kai Zimmer (fondateur). Équipe : Kai (fondateur), Pallavi (finance), Riya (opérations), Arsh (développement), Raj (développement). Contact : mint@schallern.io.

## 12. Technologie

- **Jeu :** 3D temps réel Three.js, physique de pièce déterministe sur mesure, personnages riggés avec animation faciale, télémétrie pour l’équilibrage. Les résultats des modes compétitifs seront calculés côté serveur.
- **Stack de mint :** Metaplex Core, Core Candy Machine, Umi SDK, Arweave via Irys, Helius RPC, un signataire backend Node, multisig Squads.
- **Site web :** schallern.io (anglais d’abord, allemand), pages légales sur schallern.io/legal.html.

## 13. Communauté et récompenses

Discord : https://discord.gg/FpZ5zDjV4. Les testeurs de la démo gagnent des bons de crédit de jeu pour un feedback qualifié, pour avoir rejoint Discord et pour les niveaux communautaires (plafonnés par personne ; utilisables uniquement au lancement en argent réel ; non encaissables). Les créateurs gagnent via le Programme créateurs. Règles : schallern.io/legal.html#rewards et #partners.

## 14. Risques

Schallern est en développement. La démo peut changer, la collection peut être retardée, les réseaux blockchain et les wallets peuvent tomber en panne, les objets de collection numériques peuvent perdre de la valeur, et le jeu en argent réel dépend de licences qui ne sont pas encore en place. N’achète que ce que tu peux te permettre de conserver pour lui-même.

## 15. Mentions légales et versions

Le cadre juridique, les conditions, la confidentialité et les avertissements sont tenus à jour par Culturetek Pte. Ltd. et publiés sur https://schallern.io/legal.html. Ce document est informatif, il ne constitue ni une offre de vente de titres ni un conseil en investissement. Les versions de ce whitepaper sont publiées avec leur date sur schallern.io/whitepaper/ et dans le dépôt public qui y est lié.

- v0.1 · 16 octobre 2026 · premier projet de travail
