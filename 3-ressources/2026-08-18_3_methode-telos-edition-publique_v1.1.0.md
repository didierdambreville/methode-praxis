# Méthode **TELOS**
## Cadre intégratif de conduite de projet — adaptable, observable, systémique

**Auteur :** D. Dambreville
**Version :** 1.1 — édition publique
**Date :** 18 août 2026
**Nature :** Synthèse méthodologique construite par intégration critique du corpus théorique de la gestion de projets

---

## Avertissement épistémologique

Ce document ne présente pas un standard officiel. Il propose une **architecture d'intégration** des principaux corpus théoriques — normatif (PMI, ISO, AXELOS), cybernétique, cognitif, lean, complexité, sûreté et réalisation des bénéfices — en un dispositif unique, cohérent et opérable.

Trois précautions s'imposent d'emblée.

**Première précaution.** Aucune méthode ne garantit la réussite d'un projet. Ce qu'une méthode rigoureuse produit, c'est une **réduction de la variance** des résultats : elle diminue la fréquence des échecs catastrophiques et raccourcit le délai de détection des dérives. Elle ne transforme pas un objectif erroné en succès.

**Deuxième précaution.** La sophistication méthodologique a un coût. Toute strate de processus consomme de l'attention, ressource rare et non renouvelable. Un dispositif « complet » appliqué indistinctement est, par construction, **inefficient**. C'est pourquoi le cœur de TELOS n'est pas un catalogue de pratiques mais un **moteur de contingence** qui détermine lesquelles activer.

**Troisième précaution.** Les échecs récurrents de la discipline ne relèvent pas de l'ignorance technique. Les travaux de Flyvbjerg, de Kahneman et de Lovallo établissent qu'ils procèdent de **biais cognitifs systématiques** et d'**incitations perverses**. Une méthode efficace est donc d'abord un dispositif contre-biais et contre-incitatif ; l'ordonnancement et le contrôle ne viennent qu'ensuite.

---

## Table des matières

1. [Les six thèses fondatrices](#1-les-six-thèses-fondatrices)
2. [Architecture générale de TELOS](#2-architecture-générale-de-telos)
3. [Strate **T** — Téléologie : la finalité avant l'ouvrage](#3-strate-t--téléologie--la-finalité-avant-louvrage)
4. [Strate **E** — Évaluation de contingence : le moteur d'adaptabilité](#4-strate-e--évaluation-de-contingence--le-moteur-dadaptabilité)
5. [Strate **L** — Logique d'exécution : structure, flux et engagement](#5-strate-l--logique-dexécution--structure-flux-et-engagement)
6. [Strate **O** — Observabilité : l'instrumentation du pilotage](#6-strate-o--observabilité--linstrumentation-du-pilotage)
7. [Strate **S** — Systémique : rétroaction, résilience, soutenabilité](#7-strate-s--systémique--rétroaction-résilience-soutenabilité)
8. [Le référentiel des pièges reconnus et de leurs contre-mesures](#8-le-référentiel-des-pièges-reconnus-et-de-leurs-contre-mesures)
9. [La cadence opératoire](#9-la-cadence-opératoire)
10. [Adaptation à la réalité de notre époque](#10-adaptation-à-la-réalité-de-notre-époque)
11. [Compression à petite échelle](#11-compression-à-petite-échelle)
12. [Limites et modes de défaillance de TELOS](#12-limites-et-modes-de-défaillance-de-telos)
13. [Ancrage bibliographique et corpus complémentaire](#13-ancrage-bibliographique-et-corpus-complémentaire)
14. [Annexes opératoires](#14-annexes-opératoires)

---

## 1. Les six thèses fondatrices

### Thèse I — Le projet est un moyen, jamais une fin

La conformité au triptyque coût-délai-périmètre n'est pas un critère de succès mais une **contrainte de ressources**. Un projet livré à l'heure et au budget qui ne produit aucun bénéfice est un échec dispendieux ; un projet dépassé de trente pour cent qui transforme durablement la position d'une organisation est une réussite. Cette inversion, portée par la littérature de la *benefits realisation management* (Ward et Daniel, Bradley) et par les travaux de Shenhar et Dvir, commande toute l'architecture : la mesure ultime est le **bénéfice réalisé et vérifié**, situé en aval de la livraison, souvent plusieurs mois après la clôture nominale.

Conséquence opératoire directe : aucun projet n'est clos tant que ses bénéfices n'ont pas été mesurés.

### Thèse II — Il n'existe pas de méthode universelle : loi de la variété requise

La loi d'Ashby énonce qu'un dispositif de régulation ne peut maîtriser un système que si sa propre variété égale au moins celle du système régulé. Transposée : **le degré de formalisation du pilotage doit être proportionné à la complexité et à l'incertitude de l'objet piloté**, ni plus, ni moins.

La sur-régulation d'un projet simple gaspille ; la sous-régulation d'un système de systèmes produit la catastrophe. La querelle stérile entre approches prédictives et agiles se dissout dès lors qu'on la reformule en question de calibrage. TELOS n'arbitre pas ce débat : il l'instrumente par un diagnostic préalable (strate E).

### Thèse III — L'incertitude ne se supprime pas, elle s'ordonne

Quatre régimes distincts, appelant quatre réponses irréductibles :

| Régime | Nature | Réponse appropriée | Erreur de traitement fréquente |
|---|---|---|---|
| **Risque** | Événement identifié, probabilisable | Registre, provision, assurance, mitigation | Traiter par simple provision ce qui relève de l'incertitude |
| **Incertitude** | Variabilité connue, non probabilisable finement | Tampon agrégé, marge, scénarios | Illusion de précision par le calcul probabiliste |
| **Ambiguïté** | Le cadrage lui-même est contesté | *Sensemaking*, confrontation des parties prenantes, prototypage | Trancher administrativement un désaccord de sens |
| **Ignorance** | Inconnues non identifiées | Résilience, options réelles, redondance, capacité de détection rapide | Prétendre l'avoir couverte par le registre des risques |

La faute méthodologique la plus répandue consiste à traiter les quatre régimes avec l'unique outil du registre de risques.

### Thèse IV — Un plan non instrumenté est une fiction

Un engagement dont l'avancement ne peut être observé par une source de données **indépendante du déclarant** n'est pas un engagement : c'est une déclaration d'intention. L'observabilité n'est pas un raffinement de gouvernance, c'est la condition de validité du pilotage.

Mais toute métrique érigée en cible cesse d'être une bonne métrique (loi de Goodhart). D'où l'exigence corrélative d'un **panier contradictoire** d'indicateurs : chaque signal de vitesse doit être contrebalancé par un signal de qualité, chaque signal d'avancement par un signal de valeur.

### Thèse V — L'organisation produit ce que son architecture sociale autorise

La loi de Conway — la structure d'un système reproduit la structure de communication de l'organisation qui l'a conçu — n'est pas une curiosité informatique. C'est un principe général de conception : **découper l'organisation est un acte d'ingénierie**, aussi déterminant que le découpage technique. Toute frontière organisationnelle deviendra une frontière dans le produit, et toute interface mal gouvernée entre équipes deviendra un défaut d'intégration.

### Thèse VI — Le pilotage doit distinguer le signal du bruit

L'enseignement de Shewhart et de Deming s'applique intégralement au projet : réagir à une variation de cause commune — c'est-à-dire au bruit statistique normal du système — **dégrade** la performance au lieu de l'améliorer. C'est le phénomène du *tampering*, démontré par l'expérience de l'entonnoir. Un dispositif de pilotage mature établit d'abord les limites naturelles de variation de ses indicateurs, puis ne déclenche d'action correctrice qu'en cas de franchissement caractérisé.

---

## 2. Architecture générale de TELOS

L'acronyme désigne les cinq strates du dispositif, dont l'ordre est **logiquement contraignant** : chacune conditionne la suivante.

```
   ┌──────────────────────────────────────────────────────────────┐
   │  T — TÉLÉOLOGIE                                              │
   │  Pourquoi ? Quel bénéfice, pour qui, mesuré comment,          │
   │  et à quelles conditions abandonnons-nous ?                   │
   └───────────────────────────┬──────────────────────────────────┘
                               ▼
   ┌──────────────────────────────────────────────────────────────┐
   │  E — ÉVALUATION DE CONTINGENCE                               │
   │  Quelle est la nature de cet objet ? Diagnostic à six axes    │
   │  → détermine la posture et le niveau de formalisation         │
   └───────────────────────────┬──────────────────────────────────┘
                               ▼
   ┌──────────────────────────────────────────────────────────────┐
   │  L — LOGIQUE D'EXÉCUTION                                     │
   │  Structure du travail · interfaces · flux · engagement        │
   │  temporel · gouvernance des décisions · financement           │
   └───────────────────────────┬──────────────────────────────────┘
                               ▼
   ┌──────────────────────────────────────────────────────────────┐
   │  O — OBSERVABILITÉ                                            │
   │  Instrumentation · panier contradictoire · seuils ·           │
   │  assurance indépendante · détection précoce                   │
   └───────────────────────────┬──────────────────────────────────┘
                               ▼
   ┌──────────────────────────────────────────────────────────────┐
   │  S — SYSTÉMIQUE                                               │
   │  Boucles de rétroaction simple / double / triple ·            │
   │  résilience · apprentissage · clôture et bénéfices            │
   └───────────────────────────┬──────────────────────────────────┘
                               │
                               └──── rétroaction vers T, E, L, O
```

**Axes transverses**, présents dans les cinq strates : conformité réglementaire, sécurité et cyber-résilience, soutenabilité environnementale, éthique et intégrité de l'information.

La circularité est essentielle : la strate S ne clôt pas le dispositif, elle le réalimente. Un projet qui ne modifie pas les hypothèses de la strate T à l'issue de ses premières boucles d'apprentissage n'apprend pas.

---

## 3. Strate **T** — Téléologie : la finalité avant l'ouvrage

### 3.1 L'énoncé de bénéfice

Avant toute planification, l'organisation doit produire un énoncé de bénéfice satisfaisant six critères cumulatifs :

1. **Attribution** — quel acteur précis retire quel avantage précis ?
2. **Mesurabilité** — par quelle grandeur, mesurée avec quel instrument existant ?
3. **Ligne de base** — quelle est la valeur actuelle de cette grandeur ? *Sans mesure initiale, aucun bénéfice ne pourra jamais être établi.*
4. **Profil temporel** — selon quelle courbe le bénéfice se matérialise-t-il ? Immédiat, différé, cumulatif, en escalier ?
5. **Chaîne causale** — par quel enchaînement de mécanismes la livraison produit-elle le bénéfice ? Chaque maillon est une hypothèse falsifiable.
6. **Coût d'opportunité** — que renonçons-nous à faire en engageant ces ressources ?

Le sixième critère est presque toujours omis. Il est pourtant le seul qui rende la décision d'engagement comparative, donc rationnelle.

### 3.2 La carte des bénéfices

La chaîne causale se formalise en une **carte de bénéfices** dirigée :

> Livrables → Capacités nouvelles → Changements de comportement → Bénéfices → Objectif stratégique

L'utilité de cette carte est double. Elle rend visible que la majorité des bénéfices dépend de **changements de comportement** qui ne sont pas produits par le projet lui-même — d'où l'échec massif des projets techniquement réussis mais organisationnellement non adoptés. Et elle identifie les maillons faibles, c'est-à-dire les hypothèses qu'il faut tester en priorité.

### 3.3 Les critères d'abandon, énoncés *avant* l'engagement

C'est la disposition la plus contre-intuitive et la plus puissante du dispositif. Il s'agit de formuler, **au moment de l'engagement initial**, les conditions objectives qui commanderaient l'arrêt du projet :

- seuils de dérive coût ou délai déclenchant un réexamen intégral ;
- hypothèses critiques dont l'invalidation rend la chaîne causale caduque ;
- signaux externes (concurrence, réglementation, technologie) rendant le bénéfice obsolète ;
- date-butoir de démonstration de faisabilité.

**Fondement théorique.** L'escalade d'engagement — persistance irrationnelle dans une voie défaillante — se nourrit du fait que le décideur qui devrait arrêter est celui qui a engagé. Prédéfinir les critères sépare le jugement du moment de l'engagement de celui du moment de la décision d'arrêt, neutralisant partiellement le biais des coûts irrécupérables et la dissonance cognitive.

**Disposition complémentaire.** Faire porter la décision d'arrêt par une instance distincte du promoteur du projet. Le promoteur argumente ; il ne tranche pas.

### 3.4 La contre-mesure à la représentation stratégique

Flyvbjerg distingue l'optimisme — biais involontaire — de la **représentation stratégique**, sous-estimation délibérée des coûts et surestimation des bénéfices destinée à obtenir l'approbation. Le second phénomène ne se corrige pas par de meilleures méthodes d'estimation, puisqu'il ne procède pas d'une erreur mais d'une incitation.

Trois contre-mesures structurelles :

- **Traçabilité nominative** des engagements initiaux, conservés et confrontés aux résultats à la clôture ;
- **Estimation par un tiers indépendant** du porteur, pour tout engagement au-delà d'un seuil ;
- **Alignement des incitations** : la reconnaissance porte sur le bénéfice réalisé, non sur l'obtention du financement.

---

## 4. Strate **E** — Évaluation de contingence : le moteur d'adaptabilité

C'est le cœur différenciant de TELOS. Le diagnostic étend le modèle du « diamant » de Shenhar et Dvir (nouveauté, technologie, complexité, rythme) de deux axes rendus indispensables par les conditions contemporaines : **régulation** et **irréversibilité**.

### 4.1 Le diagnostic à six axes

| Axe | Niveau 1 | Niveau 2 | Niveau 3 | Niveau 4 |
|---|---|---|---|---|
| **N — Nouveauté** (pour le marché) | Dérivé d'un existant | Amélioration de plateforme | Rupture d'usage | Inédit au monde |
| **T — Technologie** | Entièrement éprouvée | Majoritairement éprouvée | Nouvelle pour l'organisation | À inventer ou non stabilisée |
| **C — Complexité** | Composant isolé | Assemblage | Système intégré | Système de systèmes, multi-acteurs |
| **P — Rythme** | Régulier | Concurrentiel | Critique (date immuable) | Urgence vitale |
| **R — Régulation** | Aucune contrainte | Contraintes internes | Cadre réglementaire sectoriel | Sûreté, santé, données sensibles, agrément préalable |
| **I — Irréversibilité** | Décision réversible à coût nul | Réversible à coût modéré | Réversible à coût prohibitif | Strictement irréversible |

### 4.2 Les règles de conséquence

Chaque axe, au-delà du niveau 2, **impose** des dispositions. Elles ne sont pas facultatives et ne se compensent pas entre elles.

**Nouveauté ≥ 3** — Le périmètre n'est pas une donnée mais une hypothèse. Interdiction d'engagement contractuel sur un périmètre ferme. Budget d'apprentissage explicitement isolé du budget de réalisation. Cycles courts de confrontation au réel, avec des utilisateurs véritables et non des mandataires.

**Technologie ≥ 3** — Multiplier les boucles conception-test ; au minimum deux cycles de prototypage avant tout engagement de série. Réserve technique dédiée, distincte de la réserve de gestion. Ne jamais placer l'intégration en fin de séquence : la littérature établit que la phase d'intégration est le lieu privilégié de la sous-estimation.

**Complexité ≥ 3** — Formaliser les interfaces par une matrice de structure de conception (*Design Structure Matrix*), qui rend visibles les couplages et les boucles de dépendance. Instaurer une fonction de coordination dédiée, distincte de la fonction de contrôle. Contractualiser les interfaces entre lots, y compris internes.

**Rythme ≥ 3** — La latence décisionnelle devient la contrainte dominante. Déléguer par mandat écrit avec bornes explicites. Escalade en heures, non en semaines. Règle d'arbitrage préétablie : sacrifier le périmètre avant la qualité, la qualité avant la date, ou l'ordre inverse — mais l'ordre doit être fixé **avant** la crise.

**Régulation ≥ 3** — La conformité devient une exigence non fonctionnelle de premier rang, intégrée dès la strate T et non ajoutée en fin de parcours. Traçabilité documentaire des décisions. Point de contrôle réglementaire à chaque jalon. Provision de délai spécifique pour les procédures d'agrément, notoirement sous-estimées.

**Irréversibilité ≥ 3** — Le poids du jalon décisionnel doit être proportionné. Revue contradictoire obligatoire avec avocat du diable mandaté. Recherche systématique d'un dispositif de réversibilité partielle (déploiement progressif, phase pilote, architecture permettant le retour arrière) avant tout engagement définitif.

### 4.3 Détermination de la posture

Le profil des six axes détermine une posture dominante, qui n'est pas une méthodologie mais un **mode de gestion de l'incertitude**.

| Posture | Profil caractéristique | Logique | Unité d'engagement |
|---|---|---|---|
| **P1 — Prédictive tendue** | N1-2, T1-2, C3-4, R3-4 | Le connu doit être exécuté sans faute ; l'erreur est coûteuse | Lot de travail contractualisé |
| **P2 — Itérative empirique** | N3-4, T2-3, C1-2 | L'objet se découvre en le construisant | Incrément validé par usage réel |
| **P3 — Incrémentale de plateforme** | N2, T2, C2-3, flux continu | Capacité durable enrichie par ajouts | Flux de valeur, équipe permanente |
| **P4 — Exploratoire optionnelle** | N4, T4, I1-2 | Acheter de l'information avant d'acheter la réalisation | Option réelle, jalon d'abandon |
| **P5 — Hybride stratifiée** | Profils hétérogènes | Cadre prédictif englobant, poches itératives localisées | Double : jalon externe, incrément interne |

**Observation d'importance pratique :** la posture P5 correspond à la majorité des situations réelles. Les projets homogènes sont l'exception ; les référentiels les traitent pourtant comme la norme. La faute méthodologique la plus fréquente consiste à imposer une posture unique à un ensemble hétérogène — soit en soumettant une exploration à un plan détaillé, soit en confiant une intégration réglementée à une équipe sans cadre.

**Règle de stratification :** dans un projet P5, le diagnostic à six axes doit être conduit **par lot**, non globalement. Le cadre externe adopte la posture du lot le plus contraint ; chaque lot conserve en interne la posture correspondant à son propre profil.

### 4.4 Révision du diagnostic

Le diagnostic n'est pas un acte inaugural définitif. Il est **réévalué à chaque jalon majeur**, car les axes évoluent : une technologie se stabilise, une réglementation se durcit, une complexité se révèle supérieure à l'estimation initiale. Une révision d'axe déclenche mécaniquement une révision de la posture et du dispositif.

---

## 5. Strate **L** — Logique d'exécution : structure, flux et engagement

### 5.1 Décomposition duale

TELOS impose deux décompositions parallèles, dont la confrontation est féconde :

- **L'arbre de produit** (que construisons-nous ?) — décomposition par livrables et composants, stable, orientée intégration ;
- **L'arbre de bénéfices** (que produisons-nous comme effet ?) — issu de la carte de la strate T.

Tout élément de l'arbre de produit qui ne se rattache à aucune branche de l'arbre de bénéfices est un **candidat à la suppression**. C'est le mécanisme le plus efficace de contrôle du périmètre, car il opère par la justification et non par la négociation.

L'arbre de tâches — structure de découpage du travail ou carnet de commandes — dérive de ces deux arbres ; il ne les précède jamais.

### 5.2 Interfaces et dépendances

Les projets complexes échouent aux jointures, non dans les lots. La matrice de structure de conception recense les dépendances entre éléments et révèle trois configurations :

- **dépendances séquentielles** — ordonnancement simple ;
- **dépendances parallèles** — coordination légère ;
- **dépendances couplées** (boucles mutuelles) — foyer principal du risque, exigeant soit une co-localisation des responsabilités, soit une itération explicite, soit un découplage architectural.

Toute dépendance externe fait l'objet d'un **suivi d'âge** : le temps écoulé depuis la formulation de la demande. L'ancienneté d'une dépendance non résolue est un indicateur avancé de dérive infiniment plus fiable que le pourcentage d'avancement déclaré.

### 5.3 Le flux et la maîtrise de l'encours

Trois principes issus de la théorie des files d'attente et des travaux de Reinertsen :

**Loi de Little.** Le délai moyen de traversée égale l'encours divisé par le débit. Il en résulte que **réduire l'encours réduit le délai** sans aucun gain de productivité. C'est le levier le moins coûteux et le plus systématiquement ignoré.

**Réduction de la taille des lots.** Les petits lots accélèrent la rétroaction, réduisent le risque unitaire, lissent la charge et diminuent le coût de la reprise. La contrepartie est un surcoût de transaction — d'où la règle : réduire la taille des lots **jusqu'au point où le coût de transaction devient limitant**, puis attaquer ce coût lui-même par l'automatisation.

**Coût du délai.** La priorisation rationnelle ne se fonde ni sur la valeur seule, ni sur l'effort seul, mais sur le rapport du coût du délai à la durée. Un élément de valeur modérée mais rapide et à forte urgence prime sur un élément de valeur élevée mais lent et non urgent.

**Limitation explicite de l'encours.** Le multitâche organisationnel produit un effondrement du débit par accumulation des coûts de commutation. Une limite d'encours par équipe, contraignante et visible, est la disposition la plus efficiente du dispositif — coût de mise en œuvre nul, effet immédiat.

### 5.4 Estimation et engagement temporel

**Prohibition de l'estimation ponctuelle.** Toute estimation s'exprime en intervalle assorti d'un degré de confiance. Un chiffre unique est une fiction de précision qui produira de l'ancrage.

**Triangulation obligatoire.** Quatre méthodes indépendantes, dont les écarts sont eux-mêmes informatifs :
1. ascendante, par agrégation des lots ;
2. analogique, par comparaison à des réalisations passées ;
3. paramétrique, par modèle de coût ;
4. **par classe de référence**.

**La prévision par classe de référence.** C'est la contre-mesure établie au biais de planification. Le principe, issu de Kahneman et Lovallo et systématisé par Flyvbjerg, consiste à abandonner la « vue de l'intérieur » — l'analyse détaillée du cas présent, structurellement optimiste — au profit de la « vue de l'extérieur » : identifier la classe de projets comparables, établir la distribution empirique de leurs dérives, et positionner le projet présent dans cette distribution.

En l'absence de données internes, il convient de recourir aux distributions publiques sectorielles, puis de constituer progressivement une base interne. **Cette constitution est un investissement méthodologique de premier rang** : elle est la seule qui améliore structurellement la qualité prévisionnelle d'une organisation dans la durée.

**Tampons agrégés et non locaux.** L'apport de la chaîne critique de Goldratt reste sous-exploité. Lorsque chaque tâche porte sa propre marge, deux mécanismes détruisent cette marge : le syndrome de l'étudiant — le travail commence à la dernière échéance possible — et la loi de Parkinson — le travail occupe tout le temps disponible. Les marges locales ne se cumulent donc jamais ; elles se dissipent.

La disposition correcte : estimer les tâches à leur durée médiane, sans marge individuelle, retirer les dates de fin locales, et concentrer les marges retirées en **tampons agrégés** — tampon de projet en fin de chaîne critique, tampons d'alimentation aux jonctions, tampon de capacité sur les ressources contraintes. Le taux de consommation de ces tampons devient l'indicateur de santé central.

### 5.5 Gouvernance des décisions

**Droits de décision explicites.** Pour chaque catégorie de décision : qui propose, qui est consulté, qui tranche, qui est informé, et sous quel délai maximal. L'ambiguïté des droits de décision est la première cause de latence.

**Principe de subsidiarité.** La décision est prise au niveau le plus bas disposant de l'information suffisante. Toute remontée est un aveu de défaut de mandat ou de défaut d'information.

**Registre des décisions.** Chaque décision structurante est consignée : contexte, options écartées, motif, hypothèses sous-jacentes, conditions de réexamen. Ce registre est l'organe de mémoire du projet. Il permet, lorsqu'une hypothèse s'invalide, de retrouver immédiatement quelles décisions doivent être rouvertes — capacité que ni un compte rendu de réunion ni un diagramme de Gantt ne procurent.

**Financement par tranches.** Le financement intégral en une fois supprime toute option d'arrêt et engendre l'escalade. Le financement séquencé par jalons, chaque tranche conditionnée à la levée d'incertitudes déterminées, transforme la décision d'investissement en portefeuille d'options réelles. La valeur de cette structure croît avec l'incertitude.

---

## 6. Strate **O** — Observabilité : l'instrumentation du pilotage

### 6.1 Les quatre principes d'instrumentation

**Principe d'indépendance de la source.** Tout indicateur doit provenir d'une source distincte de l'acteur dont il mesure la performance. L'avancement auto-déclaré n'est pas une mesure, c'est une opinion.

**Principe de contradiction.** Les indicateurs vont par paires antagonistes. Vitesse et qualité. Avancement et valeur. Coût et dette technique. Débit et santé de l'équipe. La mesure d'une dimension seule garantit son optimisation au détriment des autres — application directe de la loi de Goodhart.

**Principe de parcimonie.** Un tableau de bord de trente indicateurs n'est pas observé. Sept à neuf signaux, hiérarchisés, avec seuils préétablis.

**Principe de discrimination statistique.** Chaque indicateur possède des limites naturelles de variation, établies empiriquement. Aucune action corrective n'est déclenchée à l'intérieur de ces limites.

### 6.2 Le panier d'indicateurs

**Signaux avancés — annonciateurs, sans attendre la matérialisation de l'écart**
- Taux de validation des hypothèses critiques (hypothèses testées sur hypothèses formulées)
- Latence décisionnelle médiane (délai entre saisine et arbitrage)
- Âge des dépendances externes non résolues
- Nombre d'hypothèses invalidées non répercutées sur le plan

**Signaux de flux**
- Encours en cours (nombre d'éléments engagés non terminés)
- Délai de traversée médian et son neuvième décile
- Débit (éléments achevés par période)
- Ratio de temps bloqué sur temps de traversée
- Âge des éléments en cours — indicateur supérieur à la vélocité, car il révèle les enlisements

**Signaux d'engagement (valeur acquise)**
- Indice de performance des coûts
- **Avancement au calendrier acquis** (*earned schedule*) plutôt que l'indice classique de délai, dont la convergence artificielle vers l'unité en fin de projet est un défaut établi
- Indice de performance à achever, comparé à la performance historique : un écart supérieur à dix pour cent signale un plan de rattrapage irréaliste

**Signaux de tampon**
- Taux de consommation des tampons rapporté à l'avancement de la chaîne critique, représenté en graphique de fièvre. C'est le meilleur indicateur composite disponible, car il intègre naturellement coût, délai et variabilité.

**Signaux de qualité**
- Taux de défauts échappés en aval
- Ratio de reprise sur travail total
- Dette technique reconnue et provisionnée

**Signaux de valeur**
- Bénéfices réalisés rapportés au profil prévu
- Coût du délai consommé depuis l'engagement

**Signaux humains**
- Mesure de sécurité psychologique par sondage court et anonyme
- Charge et rotation des personnes clés
- Volume de signaux faibles remontés spontanément — un volume en baisse est un signal d'alarme, non de santé

**Méta-signal — l'indice de divergence.** Écart mesuré entre le statut déclaré par les responsables et l'état reconstitué à partir des données objectives. Un écart persistant caractérise le syndrome dit « de la pastèque » — vert en surface, rouge à l'intérieur —, qui est le mode de défaillance dominant de la gouvernance de projet. **C'est le seul indicateur qui mesure la fiabilité du dispositif de mesure lui-même.**

### 6.3 L'assurance indépendante

Au-delà d'un seuil de complexité, d'irréversibilité ou de régulation (axes C, I ou R ≥ 3), une fonction d'assurance distincte de la ligne opérationnelle procède à des revues périodiques. Son mandat n'est pas de contrôler la conformité procédurale — exercice de faible rendement — mais de répondre à trois questions :

1. Les hypothèses fondatrices de la strate T tiennent-elles encore ?
2. Les données de la strate O sont-elles fiables et non filtrées ?
3. Un observateur extérieur, ignorant l'historique, engagerait-il aujourd'hui ce projet ?

La troisième question est la formulation opérationnelle du test des coûts irrécupérables.

---

## 7. Strate **S** — Systémique : rétroaction, résilience, soutenabilité

### 7.1 Les trois boucles d'apprentissage

La distinction d'Argyris et Schön structure toute la strate.

| Boucle | Question | Fréquence | Instance |
|---|---|---|---|
| **Simple** | Faisons-nous correctement ce que nous avons prévu ? | Hebdomadaire | Équipe |
| **Double** | Ce que nous avons prévu est-il encore pertinent ? Nos hypothèses tiennent-elles ? | Mensuelle ou par jalon | Direction de projet + commanditaire |
| **Triple** | Notre manière même de décider et de gouverner est-elle adéquate ? | Trimestrielle ou par incident majeur | Gouvernance |

**Le défaut structurel de la pratique courante est l'enfermement dans la boucle simple.** Les organisations excellent à corriger les écarts au plan et échouent à remettre le plan en question. Le dispositif doit donc **forcer** l'ouverture de la double boucle par une inscription au calendrier, indépendamment de tout déclencheur — car le déclencheur naturel, l'échec manifeste, arrive trop tard.

### 7.2 Modèle de viabilité de la gouvernance

Le modèle du système viable de Beer fournit une grille de contrôle de complétude de la gouvernance. Cinq fonctions doivent exister et être identifiables :

1. **Opérations** — les équipes qui produisent ;
2. **Coordination** — la résolution des interférences entre équipes ;
3. **Contrôle et optimisation** — l'allocation des ressources et la maîtrise de la performance ;
4. **Intelligence** — la veille sur l'environnement extérieur et l'anticipation ;
5. **Identité** — la définition de la finalité et des règles.

**Diagnostic de carence le plus fréquent : la fonction 4 est absente.** Les gouvernances de projet sont massivement tournées vers l'intérieur, régulant l'écart au plan tout en ignorant que l'environnement qui justifiait le plan s'est déplacé. C'est le mécanisme précis par lequel des projets parfaitement exécutés livrent des produits devenus inutiles.

### 7.3 Résilience et organisation attentive

Les cinq principes des organisations à haute fiabilité (Weick et Sutcliffe) se transposent intégralement :

- **Préoccupation de l'échec** — traiter tout incident mineur comme le symptôme d'une faiblesse systémique. Une baisse du nombre de signalements est une dégradation, non une amélioration.
- **Réticence à simplifier** — se méfier des explications univoques et des tableaux de bord tricolores qui écrasent la nuance.
- **Sensibilité aux opérations** — les dirigeants doivent avoir un accès direct au travail réel, non filtré par la chaîne de reporting.
- **Engagement envers la résilience** — investir dans la capacité de rétablissement autant que dans la prévention, puisque toutes les défaillances ne sont pas prévisibles.
- **Déférence à l'expertise** — en situation critique, l'autorité migre vers la compétence, non vers le rang.

L'apport de Hollnagel complète : étudier systématiquement **ce qui fonctionne** et pourquoi, et non uniquement ce qui a échoué. Les ajustements permanents par lesquels les équipes compensent les défauts du système constituent le gisement d'apprentissage le plus riche — et le moins exploité.

### 7.4 Clôture et vérification des bénéfices

La clôture d'un projet comporte trois actes, dont seul le premier est habituellement accompli :

1. **Clôture administrative** — soldes contractuels, archivage, libération des ressources ;
2. **Transfert d'exploitation** — passage à l'organisation qui exploitera l'ouvrage, avec transmission de la dette technique et des risques résiduels, formellement acceptés ;
3. **Vérification des bénéfices** — mesure effective, à six et douze mois, des grandeurs définies en strate T, comparaison au profil prévu, et **enregistrement de l'écart dans la base de classes de référence**.

Le troisième acte est la seule opération qui améliore la capacité prévisionnelle de l'organisation. Son omission systématique explique que la performance prévisionnelle du secteur ne progresse pas malgré soixante ans de littérature.

### 7.5 Soutenabilité

Trois passifs doivent être comptabilisés, et non externalisés vers l'avenir :

- **Dette technique** — provisionnée, mesurée, avec un plan d'amortissement ;
- **Empreinte environnementale** — budget carbone du projet et de l'ouvrage sur son cycle de vie, traité comme une contrainte au même titre que le budget financier ;
- **Charge humaine** — la performance obtenue par surcharge durable est un emprunt à taux usuraire, remboursé en rotation du personnel et en perte de mémoire organisationnelle.

---

## 8. Le référentiel des pièges reconnus et de leurs contre-mesures

Ce référentiel constitue l'instrument de contrôle le plus directement opérationnel du cadre. Il se lit en revue de jalon.

| # | Piège | Mécanisme | Contre-mesure structurelle | Signal précoce |
|---|---|---|---|---|
| 1 | **Biais de planification** | Vue de l'intérieur, sous-estimation systématique | Prévision par classe de référence, majoration empirique | Estimation ascendante isolée, sans comparable |
| 2 | **Représentation stratégique** | Sous-estimation délibérée pour obtenir l'accord | Estimation par tiers indépendant, traçabilité nominative | Écart entre estimation officielle et estimation informelle |
| 3 | **Escalade d'engagement** | Coûts irrécupérables, dissonance, réputation | Critères d'abandon prédéfinis, décideur d'arrêt distinct du promoteur | Argumentaires invoquant l'investissement déjà consenti |
| 4 | **Dérive du périmètre** | Ajouts sans arbitrage de valeur | Rattachement obligatoire à l'arbre de bénéfices | Demandes sans énoncé de bénéfice |
| 5 | **Rigidité de périmètre** | Refus d'adapter malgré l'invalidation des hypothèses | Double boucle calendarisée | Aucune modification de périmètre malgré des apprentissages majeurs |
| 6 | **Syndrome de l'étudiant** | Démarrage à la dernière échéance | Suppression des dates locales, tampons agrégés | Tâches systématiquement achevées juste à l'échéance |
| 7 | **Loi de Parkinson** | Le travail occupe le temps disponible | Estimation médiane, marge centralisée | Absence totale d'avance sur les tâches |
| 8 | **Loi de Brooks** | Renforcer une équipe en retard la retarde davantage | Limitation d'encours, planification de capacité | Ajout de personnes comme réponse à un retard |
| 9 | **Rapport pastèque** | Filtrage de l'information ascendante | Sources indépendantes, indice de divergence, sécurité psychologique | Statut vert prolongé suivi d'un rouge soudain |
| 10 | **Loi de Goodhart** | La métrique-cible cesse de mesurer | Panier contradictoire d'indicateurs | Amélioration d'un indicateur isolé sans effet perceptible |
| 11 | **Loi de Conway** | L'architecture reproduit l'organisation | Concevoir l'organisation comme un artefact technique | Défauts concentrés aux frontières d'équipes |
| 12 | **Bricolage statistique** | Réaction au bruit de cause commune | Limites naturelles de variation établies | Corrections fréquentes de faible amplitude |
| 13 | **Illusion de contrôle** | Le plan détaillé tenu pour la réalité | Diagnostic de contingence, intervalles d'estimation | Diagramme de Gantt à mille lignes sur objet à forte nouveauté |
| 14 | **Biais de confirmation en revue** | Les données contraires sont écartées | Prémortem, avocat du diable mandaté, équipe adverse | Revues sans aucune objection formulée |
| 15 | **Fragmentation attentionnelle** | Multitâche, effondrement du débit | Limite d'encours contraignante | Nombre de projets simultanés par personne supérieur à deux |
| 16 | **Dépendances invisibles** | Couplages non recensés | Matrice de structure de conception, suivi d'âge | Retards attribués à des causes externes non anticipées |
| 17 | **Sous-estimation de l'intégration** | Phase terminale, non prototypée | Intégration continue, jamais reportée en fin | Aucune intégration réelle avant les derniers vingt pour cent |
| 18 | **Sophisme de la moyenne** | Planifier sur des valeurs moyennes | Distributions et scénarios, simulation | Modèles à valeur unique par variable |
| 19 | **Ancrage** | Le premier chiffre contamine tous les suivants | Estimations indépendantes avant confrontation | Convergence trop rapide des estimations |
| 20 | **Effet Ringelmann** | Dilution de la responsabilité | Propriétaire nommé et unique par élément | Éléments dont la responsabilité est collective |
| 21 | **Théâtre méthodologique** | Rituels vidés de fonction | Justifier chaque rituel par sa décision produite | Cérémonies sans décision ni changement |
| 22 | **Abandon des bénéfices** | Aucune mesure après livraison | Revue obligatoire à six et douze mois | Absence de mesure initiale rendant l'écart incalculable |
| 23 | **Amnésie organisationnelle** | Aucune capitalisation | Registre des décisions, base de classes de référence | Répétition des mêmes erreurs entre projets |
| 24 | **Cécité environnementale** | Fonction d'intelligence absente | Veille formalisée, révision périodique du diagnostic | Hypothèses de marché inchangées depuis le lancement |
| 25 | **Optimisation locale** | Chaque lot optimise au détriment du tout | Mesure au niveau du flux global, non du lot | Lots performants et ensemble en retard |
| 26 | **Inflation d'artefacts assistés** | Production automatisée non vérifiée | Propriétaire humain responsable de chaque artefact | Volume documentaire croissant, lecture décroissante |

---

## 9. La cadence opératoire

Le rythme n'est pas un accessoire : il détermine la vitesse à laquelle l'information circule et donc la capacité de correction. Chaque instance est justifiée par la **décision qu'elle produit** ; une instance qui ne produit aucune décision est supprimée.

| Fréquence | Instance | Objet | Décision produite | Durée |
|---|---|---|---|---|
| Quotidienne | Synchronisation d'équipe | Blocages, encours | Levée ou escalade de blocage | ≤ 15 min |
| Hebdomadaire | Revue de flux et de tampons | Âge des éléments, consommation des tampons, dépendances | Réallocation, arbitrage de priorité | 45–60 min |
| Bimensuelle | Démonstration au réel | Confrontation à l'usage véritable | Validation ou invalidation d'hypothèse | 60 min |
| Mensuelle | Revue de double boucle | Hypothèses de la strate T, environnement | Ajustement de périmètre, de posture ou d'objectif | 90 min |
| Trimestrielle | Revue de portefeuille et de gouvernance | Arbitrage inter-projets, triple boucle | Poursuite, réorientation, arrêt, réallocation | Demi-journée |
| Par jalon | Décision d'engagement | Levée d'incertitudes, critères d'abandon | Libération ou refus de la tranche suivante | Variable |
| Événementielle | Prémortem | Anticipation de l'échec avant engagement majeur | Dispositions préventives | 90 min |
| Événementielle | Revue d'incident sans blâme | Compréhension systémique | Modification du système, non sanction | 60–120 min |
| Annuelle | Vérification des bénéfices | Mesure des bénéfices réalisés | Enrichissement de la base de classes de référence | Variable |

**Le prémortem** mérite une mention particulière. Sa forme : réunir les parties prenantes avant l'engagement, poser comme un fait accompli que le projet a échoué dix-huit mois plus tard, et demander à chacun d'écrire individuellement, avant toute discussion collective, les causes de cet échec. Le dispositif contourne la pression de conformité et libère des inquiétudes qu'aucun tour de table ordinaire n'aurait fait émerger. Son rendement est, rapporté à son coût, le plus élevé de tout le dispositif.

---

## 10. Adaptation à la réalité de notre époque

Un cadre méthodologique conçu sur le corpus classique reste incomplet s'il ignore six déplacements contemporains.

### 10.1 Le déplacement du goulot d'étranglement par l'intelligence artificielle

L'assistance générative rend la **production d'artefacts** — code, documentation, analyses, spécifications — considérablement moins coûteuse. La contrainte se déplace mécaniquement en aval : vers la **vérification, le jugement et l'intégration**.

Trois conséquences méthodologiques :

- **Réallouer l'effort.** L'effort libéré en production doit être redéployé vers la définition des critères d'acceptation, la revue et la traçabilité — sans quoi le débit apparent augmente pendant que la qualité s'effondre silencieusement.
- **Instituer la responsabilité d'artefact.** Tout artefact généré possède un propriétaire humain nommé qui en répond. Un document plausible mais non vérifié est plus dangereux qu'un document absent, car il inspire une confiance injustifiée.
- **Requalifier l'estimation.** Les classes de référence historiques deviennent partiellement caduques pour les activités automatisables. Il convient de reconstituer des classes distinctes et de ne pas extrapoler les gains de productivité observés sur les tâches de production aux tâches d'intégration, de conception et de décision, où ils sont bien moindres.

**Sur l'estimation assistée elle-même :** un modèle de langage interrogé sur une durée reproduit les biais optimistes de son corpus d'entraînement. Il constitue un instrument acceptable de génération d'hypothèses et de recherche de comparables ; il ne constitue pas une source d'estimation.

### 10.2 Le passage du mode projet au mode produit

Le projet — organisation temporaire à finalité déterminée — reste pertinent pour les ouvrages bornés. Il devient inadapté aux capacités numériques durables, où la constitution puis la dissolution répétée d'équipes détruit la connaissance accumulée.

Le mode produit substitue au financement d'initiatives temporaires le **financement d'équipes permanentes affectées à des flux de valeur**, dont la performance se mesure aux résultats produits et non à la conformité à un plan. La posture P3 du diagnostic correspond à cette configuration.

**Critère d'arbitrage :** un ouvrage à durée de vie longue et à évolution continue relève du mode produit ; un ouvrage à finalité bornée, non évolutif, relève du mode projet. La confusion des deux — traiter une plateforme durable en succession de projets — est une source majeure de dette technique et de perte de mémoire.

### 10.3 La conformité comme exigence structurante

L'accumulation réglementaire européenne — protection des données, règlement sur l'intelligence artificielle, publication d'informations de durabilité, sécurité des réseaux, résilience opérationnelle du secteur financier — modifie qualitativement le calcul.

Ces contraintes ne s'ajoutent pas en fin de parcours sans surcoût majeur : elles déterminent des choix d'architecture. L'axe **R** du diagnostic les intègre en amont. Trois dispositions :

- **Classification préalable** de l'ouvrage au regard de chaque cadre applicable, dès la strate T ;
- **Traçabilité par conception** — la production de la preuve de conformité est une exigence fonctionnelle, non une tâche documentaire terminale ;
- **Provision de délai spécifique** pour les procédures d'agrément et d'audit, dont la durée est structurellement sous-estimée.

### 10.4 Le travail distribué et asynchrone

Lorsque la coprésence disparaît, **la documentation devient l'interface principale de coordination**. Deux conséquences :

- Le registre des décisions cesse d'être une bonne pratique pour devenir une infrastructure critique ;
- La latence décisionnelle devient l'indicateur de performance organisationnelle dominant, et doit être mesurée explicitement.

### 10.5 L'orchestration sans autorité

De plus en plus de projets s'exécutent sur des écosystèmes de partenaires, de fournisseurs de services et de plateformes tierces, sur lesquels l'organisation n'exerce aucune autorité hiérarchique. Le pilotage y repose sur l'alignement d'intérêts, la contractualisation d'interfaces et la redondance des sources — non sur le commandement. Les dépendances externes non maîtrisées deviennent le premier facteur de risque calendaire, ce qui justifie leur suivi d'âge systématique.

### 10.6 La contraction des horizons de bénéfice

L'accélération de l'obsolescence réduit la durée pendant laquelle un ouvrage produit ses bénéfices. Mécaniquement, la valeur actualisée d'un ouvrage livré tardivement s'effondre plus vite qu'autrefois. Il en résulte une **prime croissante à la livraison précoce partielle** sur la livraison tardive complète, et une pénalisation accrue des plans à horizon long. Les projets dont l'horizon de conception dépasse celui de la validité de leurs hypothèses de marché sont devenus structurellement perdants.

---

## 11. Compression à petite échelle

Un cadre qui n'est opérable qu'à grande échelle n'est pas systémique : il est bureaucratique. Voici les **huit invariants** qui doivent survivre à toute compression, y compris pour une structure d'une à cinq personnes. En deçà de ces huit, le dispositif cesse d'être une méthode.

1. **Énoncé de bénéfice avec ligne de base mesurée** — une demi-page, mais avec la mesure initiale effectivement relevée.
2. **Critères d'abandon écrits avant l'engagement** — trois lignes, datées.
3. **Diagnostic à six axes** — dix minutes, refait à chaque jalon.
4. **Limite d'encours** — au plus deux initiatives simultanées par personne. C'est la disposition à plus fort rendement et à coût nul.
5. **Un tampon unique agrégé** — pas de marge par tâche.
6. **Trois indicateurs à source automatique** — un de flux, un de qualité, un de valeur.
7. **Revue mensuelle de double boucle** — une heure, calendarisée, portant exclusivement sur la validité des hypothèses.
8. **Registre des décisions et vérification des bénéfices à six mois** — deux fichiers, tenus sans exception.

Tout le reste — matrice de dépendances, valeur acquise, assurance indépendante, instances multiples — n'est activé que si le diagnostic de contingence l'impose.

---

## 12. Limites et modes de défaillance de TELOS

L'intégrité intellectuelle commande d'exposer les faiblesses du cadre proposé.

**Le coût cognitif de la strate E.** Le diagnostic à six axes exige un jugement calibré. Mal conduit, il produit une rationalisation de la posture déjà choisie plutôt qu'une détermination. Atténuation : faire scorer les axes indépendamment par deux à trois personnes avant confrontation.

**La dépendance aux données de classe de référence.** La prévision par classe de référence est la contre-mesure la plus robuste au biais de planification, mais elle suppose des données comparables. Une organisation qui débute n'en dispose pas. Atténuation : recourir aux distributions publiques sectorielles en majorant l'incertitude, et considérer la constitution de la base interne comme un livrable de premier rang.

**Le risque de théâtre.** Toute méthode explicite peut être exécutée formellement sans être pratiquée. Le référentiel des pièges recense ce mode de défaillance à son entrée 21, mais il ne s'en prémunit pas lui-même. **Test de falsification :** si aucune revue des douze derniers mois n'a produit de décision de réorientation ou d'arrêt, le dispositif ne fonctionne pas — il est appliqué sans être opérant.

**Le risque de dilution de la responsabilité.** L'insistance systémique — les défaillances procèdent du système, non des personnes — est empiriquement fondée et nécessaire à la remontée honnête de l'information. Elle peut néanmoins servir de refuge à l'incompétence individuelle. La distinction opératoire : le **système** est responsable de la fréquence des erreurs ; l'**individu** reste responsable de leur signalement.

**La limite irréductible.** Aucune disposition méthodologique ne compense un objectif faux, une incitation perverse maintenue, ou une commande politique déguisée en projet. Une méthode révèle ces situations bien plus rapidement qu'elle ne les corrige. C'est déjà considérable — mais il faut savoir que le dispositif, appliqué à un projet dont la finalité réelle diffère de la finalité déclarée, produira d'abord un conflit, non une performance.

---

## 13. Ancrage bibliographique et corpus complémentaire

### 13.1 Correspondance entre strates et sources du corpus canonique

| Strate | Sources principales du corpus canonique |
|---|---|
| **T** | Standards PMI · ISO 21500 et 21502 · Miller & Lessard · Boutinet |
| **E** | Flyvbjerg · Wysocki · Hall · Morris, Pinto & Söderlund |
| **L** | Goldratt · Moder & Phillips · Kerzner · Highsmith, Cohn, Rubin · Giard, Midler |
| **O** | EIA-748 · ISO 21508 · Anbari, Abba · revue de littérature ASU/DOE (433 réf.) · GAO |
| **S** | Müller · Söderlund · Winch · Pinto & Slevin · Heath & Heath |
| **Pièges** | Kahneman & Lovallo · Flyvbjerg · Lovallo & Kahneman · Pickrell · Stinchcombe & Heimer |

### 13.2 Compléments substantiels aux compilations usuelles

Les bibliographies de référence de la discipline sont généralement solides sur le versant normatif et sur les mégaprojets. Elles omettent en revanche, de façon récurrente, quatre versants qui sont précisément ceux dont TELOS tire ses strates E, O et S. Les références qui suivent sont donc indispensables à qui entend mettre le cadre en œuvre.

**Contingence et théorie du projet**
- Shenhar, Aaron J., & Dvir, Dov. (2007). *Reinventing Project Management: The Diamond Approach to Successful Growth and Innovation*. Harvard Business School Press. — *Source du modèle de contingence : chaînon manquant de la plupart des compilations, alors qu'il conditionne toute démarche d'adaptation.*
- Snowden, David J., & Boone, Mary E. (2007). A Leader's Framework for Decision Making. *Harvard Business Review*. — *Cadre Cynefin.*
- Turner, J. Rodney. *The Handbook of Project-Based Management*. McGraw-Hill.
- Lundin, Rolf A., & Söderholm, Anders. (1995). A Theory of the Temporary Organization. *Scandinavian Journal of Management*.

**Flux, files d'attente et économie du développement**
- Reinertsen, Donald G. (2009). *The Principles of Product Development Flow*. Celeritas. — *Source du coût du délai, de la taille de lot et de l'économie des files d'attente ; rarement recensé hors de la littérature de développement de produit.*
- Brooks, Frederick P. (1975). *The Mythical Man-Month*. Addison-Wesley. — *Classique fondateur, curieusement absent de nombreuses compilations.*
- Forsgren, Nicole, Humble, Jez, & Kim, Gene. (2018). *Accelerate*. IT Revolution.
- Kersten, Mik. (2018). *Project to Product*. IT Revolution.

**Cybernétique, mesure et qualité**
- Ashby, W. Ross. (1956). *An Introduction to Cybernetics*. Chapman & Hall. — *Loi de la variété requise.*
- Beer, Stafford. (1979). *The Heart of Enterprise* / (1972). *Brain of the Firm*. Wiley. — *Modèle du système viable.*
- Deming, W. Edwards. (1986). *Out of the Crisis*. MIT Press.
- Wheeler, Donald J. (2000). *Understanding Variation: The Key to Managing Chaos*. SPC Press.
- Hubbard, Douglas W. (2014). *How to Measure Anything* (3e éd.). Wiley.
- Savage, Sam L. (2009). *The Flaw of Averages*. Wiley.

**Cognition, sûreté, apprentissage et bénéfices**
- Kahneman, Daniel. (2011). *Thinking, Fast and Slow*. Farrar, Straus and Giroux.
- Flyvbjerg, Bent, & Gardner, Dan. (2023). *How Big Things Get Done*. Currency. — *Synthèse la plus récente et la plus opérationnelle des travaux de Flyvbjerg.*
- Argyris, Chris, & Schön, Donald A. (1996). *Organizational Learning II*. Addison-Wesley.
- Weick, Karl E., & Sutcliffe, Kathleen M. *Managing the Unexpected* (3e éd.). Jossey-Bass.
- Hollnagel, Erik. (2014). *Safety-I and Safety-II*. Ashgate.
- Perrow, Charles. (1984). *Normal Accidents*. Basic Books.
- Edmondson, Amy C. (2018). *The Fearless Organization*. Wiley.
- Ward, John, & Daniel, Elizabeth. *Benefits Management*. Wiley. — *Le versant « réalisation des bénéfices » constitue l'angle mort le plus fréquent des bibliographies de gestion de projet.*
- Bradley, Gerald. *Benefit Realisation Management*. Gower.
- Eppinger, Steven D., & Browning, Tyson R. (2012). *Design Structure Matrix Methods and Applications*. MIT Press.
- DeMarco, Tom, & Lister, Timothy. *Peopleware* (3e éd.). Addison-Wesley.

**Normes fréquemment omises**
- **ISO 31000:2018** — *Management du risque — Lignes directrices*. *Norme de référence en gestion des risques, complément indispensable de la famille 21500 et pourtant rarement citée à ses côtés.*
- ISO/IEC 31010:2019 — *Techniques d'appréciation du risque*.
- ISO 56002 — *Management de l'innovation — Lignes directrices*, pertinente pour tout projet dont l'axe N atteint ou dépasse le niveau 3.

**Sur le corpus AXELOS :** la septième édition de *Managing Successful Projects with PRINCE2* (2023) constitue la version en vigueur ; il serait utile de la dater explicitement, l'édition étant structurellement remaniée par rapport à la précédente.

**Revues académiques de référence**
- *International Journal of Project Management* (Elsevier)
- *Project Management Journal* (PMI / SAGE)
- *International Journal of Managing Projects in Business* (Emerald)

---

## 14. Annexes opératoires

### Annexe A — Fiche de diagnostic de contingence

| Axe | Score (1–4) | Justification factuelle | Dispositions déclenchées |
|---|---|---|---|
| N — Nouveauté | | | |
| T — Technologie | | | |
| C — Complexité | | | |
| P — Rythme | | | |
| R — Régulation | | | |
| I — Irréversibilité | | | |

**Posture retenue :** ☐ P1 ☐ P2 ☐ P3 ☐ P4 ☐ P5
**Date du diagnostic :** ____ · **Prochaine révision :** ____ · **Scoré indépendamment par :** ____

### Annexe B — Checklist de lancement (douze questions)

1. Le bénéfice est-il énoncé avec un bénéficiaire nommé et une grandeur mesurable ?
2. La **ligne de base** de cette grandeur a-t-elle été effectivement mesurée ?
3. La chaîne causale entre livrable et bénéfice est-elle explicite, maillon par maillon ?
4. Quelles sont les trois hypothèses dont l'invalidation ruinerait le projet ?
5. Les critères d'abandon sont-ils écrits, datés et connus des parties prenantes ?
6. Le coût d'opportunité est-il chiffré ? À quoi renonçons-nous ?
7. Le diagnostic à six axes est-il conduit, et par plusieurs personnes indépendamment ?
8. L'estimation repose-t-elle sur au moins une classe de référence externe ?
9. Les droits de décision et les délais maximaux d'arbitrage sont-ils formalisés ?
10. Les trois indicateurs minimaux ont-ils une source de données **indépendante du déclarant** ?
11. Un prémortem a-t-il été conduit, avec écriture individuelle préalable ?
12. Le financement est-il séquencé par tranches conditionnelles ?

### Annexe C — Checklist de jalon décisionnel

1. Les hypothèses critiques ont-elles été testées ? Lesquelles sont invalidées ?
2. Le diagnostic à six axes a-t-il évolué ? La posture reste-t-elle appropriée ?
3. Quel est le taux de consommation des tampons rapporté à l'avancement ?
4. L'indice de divergence — statut déclaré contre données objectives — est-il nul ?
5. Un critère d'abandon est-il atteint ou approché ?
6. **Test de l'observateur extérieur :** en ignorant tout l'investissement déjà consenti, engagerions-nous ce projet aujourd'hui ?
7. Le bénéfice attendu a-t-il été révisé à la baisse depuis le lancement ? De combien ?
8. La tranche de financement suivante est-elle libérée, réduite, conditionnée ou refusée ?

### Annexe D — Checklist de clôture et de bénéfices

1. Clôture administrative : soldes, archivage, libération des ressources.
2. Transfert d'exploitation : dette technique et risques résiduels **formellement acceptés** par l'exploitant.
3. Rétrospective sans blâme : ce qui a fonctionné, et pourquoi — pas uniquement ce qui a échoué.
4. Écart entre estimation initiale et réalisé, **versé dans la base de classes de référence**.
5. Rendez-vous de mesure des bénéfices inscrits au calendrier à six et douze mois, avec responsable nommé.
6. Registre des décisions archivé et rendu consultable.

### Annexe E — Tableau de bord minimal

| Indicateur | Source (indépendante) | Seuil d'alerte | Contre-indicateur associé |
|---|---|---|---|
| Âge du plus ancien élément en cours | Outil de suivi | > 2× délai médian | Débit |
| Consommation de tampon / avancement | Plan | Zone rouge du graphique de fièvre | Périmètre livré |
| Ratio de reprise | Outil de suivi | > 15 % | Délai de traversée |
| Bénéfice réalisé / profil prévu | Système métier | Écart > 20 % | Coût engagé |
| Latence décisionnelle médiane | Registre des décisions | > 5 jours ouvrés | Qualité des décisions |
| Indice de divergence | Comparaison statut / données | Tout écart persistant | — |

---

## Synthèse en une page

**TELOS repose sur une inversion et cinq subordinations.**

L'**inversion** : ce n'est pas le plan qui mesure le projet, c'est le bénéfice réalisé qui mesure le plan.

Les **subordinations**, dans un ordre logiquement contraignant :

1. La **méthode** est subordonnée à la **finalité** — on ne choisit pas un cadre avant de savoir ce que l'on cherche à produire comme effet.
2. Le **niveau de formalisation** est subordonné au **diagnostic de contingence** — la variété du dispositif doit égaler celle de l'objet, ni plus, ni moins.
3. Le **plan** est subordonné à l'**observabilité** — un engagement non instrumenté par une source indépendante n'est pas un engagement.
4. Le **contrôle** est subordonné à l'**apprentissage** — corriger l'écart au plan sans jamais interroger le plan est le mode de défaillance dominant de la discipline.
5. La **performance** est subordonnée à la **soutenabilité** — la vitesse obtenue par accumulation de dette technique, environnementale ou humaine est un emprunt, non un gain.

Et un principe de conception qui les traverse toutes : **les erreurs récurrentes de la gestion de projet ne sont pas des accidents mais des produits structurels de biais cognitifs et d'incitations mal alignées.** Une méthode efficace est donc d'abord une architecture de contre-mesures — les critères d'abandon prédéfinis, la prévision par classe de référence, le prémortem, l'indice de divergence et la revue de double boucle calendarisée en constituent le noyau irréductible.

---

*Document constitué en synthèse critique du corpus référencé. Les cadres et lois mobilisés sont attribués à leurs auteurs au chapitre 13 ; l'architecture d'intégration en cinq strates, le diagnostic à six axes et le référentiel des vingt-six pièges constituent la contribution propre du présent document.*
