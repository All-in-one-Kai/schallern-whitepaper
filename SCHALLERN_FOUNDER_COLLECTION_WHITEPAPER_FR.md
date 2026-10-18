# Schallern — Whitepaper Founder Collection

**Version 0.2 · Projet de travail · 18 octobre 2026 · Culturetek Pte. Ltd., Singapour**

> Flip the World. Un lancer. Un mur. Les millimètres décident.

## 1. Résumé

Schallern est un jeu de lancer de pièces calibré physiquement, joué dans le navigateur : lance une pièce vers un mur ; la pièce dont le bord le plus proche s’immobilise le plus près du mur gagne. Le jeu est une version moderne d’un jeu de cour de récré joué avec l’argent du lait dans l’Allemagne des années 1980. Une démo gratuite et jouable avec trois arènes et trois personnages est en ligne sur https://schallern.io/play/.

La **Founder Collection** est une série prévue de **10 000 objets de collection numériques sur Solana** (pièces et personnages). Les Founder Collectibles sont cosmétiques : ils changent l’apparence de la pièce et de l’avatar d’un joueur, jamais la physique, la géométrie ou les chances. Le mint finance la prochaine étape de développement du jeu. Ce whitepaper décrit le jeu, la collection, la mécanique du mint, l’emploi des fonds, la roadmap et l’équipe, et distingue ce qui est en ligne aujourd’hui de ce qui est prévu.

## 2. Le jeu

**Règle.** Un mur, une pièce par lancer, trois manches par match ; le plus petit total gagne. Un lancer compte la distance en millimètres entre le bord le plus proche de la pièce et le mur, une fois la pièce immobilisée. La pièce n’a **pas** besoin de toucher le mur. Une pièce restée appuyée contre le mur (pièce appuyée, ou leaner) compte 0 mm. La caméra, les ombres et les visuels ne décident jamais d’un vainqueur ; le résultat physique le fait.

**Faute et lancers non valables.** La seule faute est une pièce qui passe par-dessus le mur. Un lancer est non valable si le premier contact de la pièce avec le sol se situe à moins de 2 m après la ligne de lancer (atterrir exactement sur la ligne des 2 m est valable). Une faute ou un lancer non valable compte pour la distance de la manche ; aucun lancer valable ne peut être compté plus mal.

**Carte de manche.** Avant chaque manche, une carte affiche les conditions, identiques pour tous les joueurs : la distance de lancer entre 6 et 10 m, en valeurs non rondes (par exemple 7,43 m), la pièce de la manche, tirée d’un catalogue de vraies pièces à leur taille réelle, ainsi que les zones visibles du sol et du mur (par exemple fissures, gravier, endroits lisses ou plaques de métal) et la pente.

**Physique.** La pièce est un disque mince doté des données de vraies pièces, simulé avec friction, résistance au roulement et rebond par surface (asphalte, sable, marbre) et par matériau de mur. Le modèle est calibré physiquement à partir de mesures publiées ; un calibrage sur de vrais lancers filmés reste à faire, c’est pourquoi nous ne parlons pas encore de physique réelle. La simulation est déterministe : la même entrée donne le même résultat sur chaque appareil.

**Commandes.** Quatre styles de lancer : Glisseur (bas et à plat), Demi-arc, Lob haut et Claque au mur, chacun avec sa propre plage de vitesse et de courbe. Appuie et tire vers l’arrière pour la puissance et la direction, courbe le geste pour donner de l’effet latéral, puis lâche pendant que l’anneau de lâcher se resserre ; le timing et une main sûre font la qualité du lâcher. Souris et tactile utilisent la même entrée normalisée.

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
- **Sujets :** pièces Schallern réparties en huit catégories de traits visibles : palier, matériau, finition, tranche, motif (dont les personnages du jeu), inscription, arrière-plan (dont 48 murs célèbres) et effet.
- **Standard :** Metaplex Core sur Solana ; chaque objet de collection est un asset on-chain dans une collection vérifiée avec des informations de royalties on-chain.
- **Rareté :** 8 catégories de traits avec 129 valeurs ; chaque pièce possède toutes les catégories et son propre rang de rareté. Paliers : 11 pièces uniques (1/1), 89 Legendary, 500 Epic, 1 400 Rare, 3 000 Uncommon et 5 000 Common. La rareté n’est que du prestige visuel.
- **Attribution aléatoire et reveal :** les acheteurs ne choisissent ni l’artwork, ni la rareté, ni le palier. Jusqu’à l’épuisement de la collection, chaque objet de collection affiche le même visuel provisoire. Avant l’ouverture du mint, un hash de provenance de la collection complète et ordonnée est publié et stocké on-chain. Une fois la collection épuisée, le décalage de départ est tiré d’un futur slot Solana annoncé à l’avance : personne, pas même l’équipe, ne peut décider qui reçoit quelle pièce. Chacun peut vérifier le résultat à l’aide du hash publié.
- **Droits sur l’artwork :** les holders peuvent utiliser commercialement l’artwork de leur objet de collection. La marque SCHALLERN (nom et logo) en est exclue et reste à l’opérateur. Le texte final de la licence est publié avec les conditions du mint.

## 5. Ce qu’un Founder reçoit, et ce qu’un Founder ne reçoit pas

**Reçoit :** l’objet de collection comme skin de lancer dans le jeu dès que la liaison du wallet est active ; un badge Founder avec le numéro de l’objet sur le profil de joueur ; le rôle Founder et les salons réservés aux holders sur Discord ; un vote sur les prochaines arènes et les prochains designs de pièces ; un accès anticipé aux nouvelles arènes en mode argent fictif ; le droit d’utiliser commercialement l’artwork (hors marque SCHALLERN).

**Ne reçoit pas :** une participation dans la société, un droit à des bénéfices, distributions, rachats ou plus-values, ni aucun avantage de gameplay. La Founder Collection est un objet de collection, pas un produit d’investissement. Tout financement de la société est une offre distincte, structurée séparément (voir section 10).

## 6. Mécanique du mint

| Élément | Plan |
|---|---|
| Chaîne et standard | Solana, Metaplex Core, une seule Core Candy Machine avec Candy Guard |
| Paliers de prix | fixés par le nombre de ventes, et non choisis par l’acheteur : #1–4 000 à 0,5 SOL · #4 001–7 000 à 1 SOL · #7 001–9 000 à 1,5 SOL · #9 001–10 000 à 2 SOL. Les premiers acheteurs paient moins ; un achat qui franchit un palier est facturé pièce par pièce (modèle prévu ; les conditions définitives sont publiées avant le lancement) |
| Attribution | artwork et rareté aléatoires pour les 10 000 pièces depuis une seule Candy Machine, révélés une fois la collection épuisée (voir section 4) |
| Phases | lancement le **11 novembre 2026 à 11 h 11 SGT (03 h 11 UTC)** ; OG → Allowlist → public ; l’Allowlist donne un accès plus tôt. Les dates et tout changement sont annoncés uniquement sur schallern.io et dans les canaux officiels Discord et Telegram |
| Limites | aucune limite par wallet, quelle que soit la phase ; protection anti-bot par captcha, contrôles de fréquence et taxe anti-bot ; chaque transaction de mint est construite et cosignée par le backend Schallern |
| Où | uniquement sur schallern.io ; l’équipe n’écrit jamais en premier et ne demande jamais de seed phrase |
| Disponibilité | le mint n’est restreint géographiquement que là où les conditions de nos prestataires l’exigent |
| Trésorerie | les produits du mint sont versés on-chain dans un coffre multisig 2 sur 3 (Squads v4) de l’opérateur ; aucune clé ne peut à elle seule déplacer les fonds |
| Royalties | 5 % de royalties sur le marché secondaire, inscrites dans la collection |
| Stockage | artwork et métadonnées sur Arweave (permanent) ; l’artwork définitif est uploadé au reveal |
| Répétition | le flux complet (collection, une seule Candy Machine avec visuel provisoire et hash de provenance on-chain, groupes de phases et de paliers de prix, signataire backend, contrôles géographiques et de sanctions, tests anti-bot et de charge, reveal à partir d’un slot Solana, vérification publique) a été exécuté et vérifié sur le devnet Solana en octobre 2026 |

Les coûts de mint pour les acheteurs sont le prix du palier en cours plus les frais de réseau Solana (environ 0,003 SOL par mint).

## 7. Emploi des fonds

Les produits financent la prochaine étape de développement de Schallern. L’allocation prévue couvre : le développement du jeu (multijoueur, tournois, comptes), l’art et l’animation (production de la collection, nouvelles arènes), l’infrastructure et la sécurité (serveurs, RPC, audits), la communauté et le marketing (Programme créateurs, événements) et une réserve d’exploitation. La répartition en pourcentage ainsi que les scénarios de financement minimum, cible et étendu sont publiés avant l’ouverture du mint. Les royalties secondaires ne font pas partie du budget de base.

## 8. Roadmap

1. **Jouable maintenant :** démo 3D, trois arènes, réglages fins avec les retours des joueurs, Programme créateurs, récompenses démo.
2. **Ensuite :** la Founder Collection, la croissance de la communauté, le concept final du mint et le mint.
3. **Prévu :** matchs en ligne, crews de ville, tournois, comptes joueurs avec récompenses et tableaux de bord d’affiliation.
4. **Vision :** figurines physiques personnelles, vrais murs, événements live.

Hormis le lancement du Founder Mint (11 novembre 2026, 11 h 11 SGT), les dates ne sont pas promises. Chaque étape est annoncée quand elle est prête.

## 9. L’économie du jeu (mode argent réel prévu)

Le jeu en argent réel est une étape ultérieure, licenciée séparément. Le modèle prévu : une table fixe la mise (par exemple six joueurs, trois manches, 1 USDC chacun) ; le vainqueur remporte le pot moins une **commission de la maison de 10 % sur le gain positif** ; les mises et les commissions de la maison sont strictement séparées. Les créateurs qui amènent des joueurs reçoivent **10 % des commissions de la maison ajustées** de leurs joueurs pendant 36 mois (voir schallern.io/partners.html). Les Founder Collectibles ne jouent aucun rôle dans cette économie, si ce n’est d’être le skin avec lequel un joueur lance.

## 10. Financement de la société (distinct de la collection)

Schallern discute également avec des investisseurs privés du financement de la société (minimum prévu : 20 000 EUR). Il s’agit d’une offre distincte et privée avec ses propres conditions et documents, accessible uniquement après candidature et examen. Elle n’est jamais couplée à la Founder Collection, et rien dans ce whitepaper n’en fait partie.

## 11. Équipe et opérateur

Opérateur jusqu’à la création de la société du jeu : **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Directeur : Kai Zimmer (fondateur). Équipe : Kai (fondateur), Pallavi (finance), Riya (opérations), Arsh (développement), Raj (développement). Contact : mint@schallern.io.

## 12. Technologie

- **Jeu :** 3D temps réel Three.js, physique de pièce sur mesure, déterministe et calibrée physiquement, personnages riggés avec animation faciale, télémétrie pour l’équilibrage. Les résultats des modes compétitifs seront calculés côté serveur.
- **Stack de mint :** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, Helius RPC, un signataire backend Node, un coffre multisig Squads v4 pour les produits.
- **Site web :** schallern.io (anglais d’abord, allemand), pages légales sur schallern.io/legal.html.

## 13. Communauté et récompenses

Discord : https://discord.gg/FpZ5zDjV4. Les testeurs de la démo gagnent des bons de crédit de jeu pour un feedback qualifié, pour avoir rejoint Discord et pour les niveaux communautaires (plafonnés par personne ; utilisables uniquement au lancement en argent réel ; non encaissables). Les créateurs gagnent via le Programme créateurs. Règles : schallern.io/legal.html#rewards et #partners.

## 14. Risques

Schallern est en développement. La démo peut changer, la collection peut être retardée, les réseaux blockchain et les wallets peuvent tomber en panne, les objets de collection numériques peuvent perdre de la valeur, et le jeu en argent réel dépend de licences qui ne sont pas encore en place. N’achète que ce que tu peux te permettre de conserver pour lui-même.

## 15. Mentions légales et versions

Le cadre juridique, les conditions, la confidentialité et les avertissements sont tenus à jour par Culturetek Pte. Ltd. et publiés sur https://schallern.io/legal.html. Ce document est informatif, il ne constitue ni une offre de vente de titres ni un conseil en investissement. Les versions de ce whitepaper sont publiées avec leur date sur schallern.io/whitepaper/ et dans le dépôt public qui y est lié.

- v0.1 · 16 octobre 2026 · premier projet de travail
- v0.2 · 18 octobre 2026 · règles du jeu de la démo V04 (toucher le mur n’est plus requis, seule faute = par-dessus le mur, ligne d’atterrissage à 2 m, carte de manche, quatre styles de lancer), formulation « calibré physiquement », attribution aléatoire avec raretés et reveal après épuisement de la collection, une seule Candy Machine, paliers de prix selon le nombre de ventes, aucune limite par wallet, système de traits et nombre de pièces par palier, usage commercial de l’artwork, restriction géographique
