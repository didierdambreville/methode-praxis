# RÉFÉRENTIEL DE CLASSIFICATION UNIFIÉE DES PROJETS
## Modèle à trois axes : SUJET × STADE × STATUT

**Version** 1.0
**Date** 2026-08-18
**Statut** Spécification ouverte
**Licence** CC BY-SA 4.0

---

## AVERTISSEMENT NORMATIF

Les termes clés **DOIT**, **NE DOIT PAS**, **DEVRAIT**, **NE DEVRAIT PAS** et **PEUT**
sont employés au sens de la RFC 2119 (Bradner, 1997) :

| Terme | Portée |
|---|---|
| **DOIT** / **NE DOIT PAS** | Exigence absolue. Une implémentation qui y déroge n'est pas conforme. |
| **DEVRAIT** / **NE DEVRAIT PAS** | Recommandation forte. Une dérogation exige une justification explicite et documentée. |
| **PEUT** | Option laissée à l'implémentation, sans effet sur la conformité. |

---

# PARTIE I — CADRE

## 1. Objet

Le présent référentiel définit un modèle de classification unique, applicable à
l'ensemble des projets d'une organisation ou d'un individu, quels que soient leur
nature, leur échelle et leur secteur.

Il vise à résoudre un problème structurel et récurrent : **la surcharge de l'arborescence**.
Dans la quasi-totalité des systèmes documentaires observables, un unique dispositif
hiérarchique — l'arbre de répertoires — est sommé de répondre simultanément à trois
questions hétérogènes :

1. *De quoi cet objet traite-t-il ?* (question du **sujet**)
2. *Où en est-il dans son cycle de production ?* (question du **stade**)
3. *Qu'en fait-on maintenant ?* (question du **statut**)

Un arbre ne peut exprimer qu'une seule de ces dimensions sans se dégrader. Le référentiel
énonce donc un principe d'**orthogonalité** et en dérive un ensemble de règles.

## 2. Domaine d'application

Le référentiel s'applique :

- à l'organisation des systèmes de fichiers, dépôts documentaires et bases de connaissances ;
- au pilotage de portefeuilles de projets, quel qu'en soit le nombre ;
- à la conduite de projets individuels, du programme pluriannuel à la tâche isolée ;
- indifféremment aux contextes professionnels, associatifs et personnels.

## 3. Hors domaine

Le référentiel **NE DOIT PAS** être considéré comme couvrant :

- les obligations légales de conservation, de sécurité ou de confidentialité, qui relèvent
  de cadres propres (ISO 15489, ISO/IEC 27001, réglementations sectorielles) et **priment** ;
- la gestion des secrets d'authentification, qui **DOIT** demeurer confiée à un
  dispositif spécialisé et **NE DOIT PAS** transiter par l'arborescence documentaire ;
- les méthodes d'estimation, de contractualisation et d'allocation budgétaire ;
- les outils : le référentiel est délibérément agnostique quant à l'implémentation.

## 4. Terminologie

| Terme | Définition retenue |
|---|---|
| **Artefact** | Toute unité d'information susceptible d'être classée : fichier, note, enregistrement, fil de discussion, actif. |
| **Axe** | Dimension indépendante de description. Trois axes sont définis : Sujet, Stade, Statut. |
| **Taxon** | Position dans l'axe du Sujet ; se matérialise par un répertoire. |
| **Stade** | Position dans le cycle de production ; se matérialise par un code numérique. |
| **Statut** | État d'attention et d'actionnabilité ; se matérialise par une valeur en registre. |
| **Registre** | Table unique recensant les objets pilotés et portant leur statut. |
| **Sas** | Zone tampon recevant les entrées non encore classées. |
| **Coordonnée** | Triplet (taxon, stade, statut) identifiant complètement un artefact. |

---

# PARTIE II — FONDEMENTS

## 5. Le problème de la surcharge d'axe

Un arbre de répertoires est une **classification énumérative** : chaque objet occupe une
position et une seule, déterminée par un chemin unique. Cette contrainte, héritée des
classifications bibliographiques du XIXe siècle et de l'organisation physique des
rayonnages, n'a plus de nécessité technique dans un environnement numérique — mais elle
survit dans les interfaces, et façonne les pratiques.

Lorsqu'un utilisateur tente de faire porter à l'arbre plusieurs dimensions simultanées,
trois dégradations apparaissent invariablement :

1. **La multiplication combinatoire.** Croiser *n* sujets et *m* stades exige *n × m*
   répertoires. Le système croît plus vite que le contenu qu'il ordonne.
2. **L'hésitation de rangement.** Un artefact relevant de deux dimensions n'a plus de
   place déterminée ; l'utilisateur arbitre au cas par cas, et cet arbitrage n'est pas
   reproductible d'une fois sur l'autre. Le classement cesse d'être une fonction.
3. **La duplication.** Faute de trancher, l'utilisateur copie. Le système perd sa source
   unique de vérité et les versions divergent silencieusement.

Ces trois pathologies ont une cause commune et une seule : **un dispositif à une
dimension chargé d'exprimer une réalité à plusieurs dimensions**.

## 6. État de l'art

### 6.1 La classification à facettes

La réponse théorique à ce problème est ancienne et parfaitement établie. Ranganathan
(*Prolegomena to Library Classification*, 1937 ; *Colon Classification*, 1933) démontre
qu'une classification énumérative ne peut couvrir un domaine évolutif sans exploser, et
propose de lui substituer une **classification à facettes** : on identifie un petit
nombre de dimensions fondamentales — sa formule canonique PMEST distingue Personnalité,
Matière, Énergie, Espace, Temps — puis on *compose* la description d'un objet à partir
d'une valeur prise dans chacune. Vickery (*Faceted Classification*, 1960) en généralise
la méthode hors du champ bibliothécaire.

Le présent référentiel est une application directe de cette doctrine, réduite à trois
facettes et adaptée à l'objet « projet ».

### 6.2 La critique des catégories classiques

Rosch (« Principles of Categorization », 1978) puis Lakoff (*Women, Fire, and Dangerous
Things*, 1987) établissent que les catégories humaines ne fonctionnent pas par conditions
nécessaires et suffisantes, mais par ressemblance à un prototype, avec des frontières
graduées. Il s'ensuit qu'aucune taxonomie ne classera jamais sans reste : **toute
classification produit des cas limites, et un système qui ne les prévoit pas se rigidifie
ou se contourne**. D'où la nécessité normative d'un sas (§ 14) et d'une règle d'arbitrage
par défaut (§ 11, N4).

Bowker et Star (*Sorting Things Out*, 1999) ajoutent une dimension politique décisive :
une classification est une infrastructure, elle devient invisible à l'usage, et elle
distribue de la visibilité — ce qu'elle ne prévoit pas cesse pratiquement d'exister.
Toute catégorie « Divers » **DEVRAIT** donc être considérée comme un signal de défaut,
non comme une commodité.

Weinberger (*Everything Is Miscellaneous*, 2007) formule le corollaire numérique : l'ordre
physique impose l'unicité de place, l'ordre numérique ne l'impose plus. On **PEUT** donc
maintenir un arbre unique *et* superposer des dimensions par métadonnées — ce que le
présent modèle fait.

### 6.3 Les méthodes de cycle

L'axe du Stade s'appuie sur les méthodes de conception qui ordonnent l'intervention sur
un milieu préexistant. La séquence **OBREDIM** — Observation, Bordures, Ressources,
Évaluation, Conception, Installation, Maintenance — issue de la tradition pédagogique de
la permaculture (Mollison, 1988 ; Holmgren, 2002), présente une propriété rare : elle
consacre quatre stades sur sept à la lecture du milieu avant toute production.

Elle rejoint, par des voies indépendantes, la méthodologie des systèmes souples de
Checkland (1981), qui refuse le problème donné d'avance ; la logique effectuale de
Sarasvathy (2001), qui fait précéder l'inventaire des moyens par la définition du but ;
et la boucle OODA de Boyd, qui partage la structure en inversant le tempo.

### 6.4 Les états documentaires

L'axe du Statut s'appuie sur deux traditions convergentes.

La **gestion de l'archivage** distingue de longue date les âges d'un document — courant,
intermédiaire, définitif — et associe à chacun un régime de conservation et une décision
de sort final (ISO 15489-1:2016 ; ISO 14721:2012, modèle OAIS). Le modèle du *records
continuum* (Upward, 1996) corrige la lecture linéaire : l'archivage n'est pas la mort
d'un document mais un changement de régime d'usage.

Les **systèmes d'organisation personnelle** ont formalisé le même constat sous une forme
opératoire. GTD (Allen, 2001) sépare l'action suivante du projet qui la porte ; PARA
(Forte, 2022) distingue quatre états — Projets, Domaines, Ressources, Archives — selon
l'horizon d'actionnabilité ; les méthodes de notes en réseau (Ahrens, 2017) posent que la
valeur d'une ressource croît avec ses liens, non avec son emplacement.

### 6.5 La séparation des préoccupations

Enfin, le principe d'orthogonalité qui structure ce référentiel est un emprunt explicite
au génie logiciel : Parnas (« On the Criteria To Be Used in Decomposing Systems into
Modules », 1972) et Dijkstra (« On the role of scientific thought », 1974) établissent
qu'un système se décompose selon les dimensions susceptibles de varier indépendamment,
et non selon les étapes de son exécution. Le sujet, le stade et le statut d'un artefact
varient indépendamment ; ils constituent donc trois modules distincts.

## 7. Principe d'orthogonalité

> **P1.** Les trois axes sont indépendants : la valeur prise sur l'un ne détermine
> aucune valeur sur les autres.
>
> **P2.** À chaque axe correspond un et un seul mécanisme de matérialisation.
>
> **P3.** Un mécanisme de matérialisation ne porte qu'un seul axe.

| Axe | Question | Mécanisme | Vitesse de variation |
|---|---|---|---|
| **SUJET** | De quoi s'agit-il ? | L'arborescence de répertoires | Très lente (années) |
| **STADE** | Où en est la production ? | Un chiffre dans le nom de l'artefact | Moyenne (semaines) |
| **STATUT** | Qu'en fait-on ? | Une valeur dans le registre | Rapide (jours) |

L'attribution des mécanismes n'est pas arbitraire : **elle suit la vitesse de variation**.
La dimension la plus stable reçoit le support le plus coûteux à modifier (l'arborescence) ;
la plus volatile reçoit le support le moins coûteux (une cellule de tableur ou un champ
de base). Inverser cette correspondance — c'est le cas de tout système qui crée des
répertoires « En cours » ou « Urgent » — garantit un travail de réorganisation permanent
et sans valeur ajoutée.

---

# PARTIE III — LE MODÈLE

## 8. Axe A — SUJET

### 8.1 Nature

L'axe du Sujet répond à la question *de quoi cet artefact traite-t-il ?* Il est
**énumératif, hiérarchique et lent**. Il constitue la seule matérialisation autorisée
sous forme de répertoires.

### 8.2 Règles

- **A1.** L'arborescence **NE DOIT** exprimer **QUE** le sujet. Aucun niveau **NE DOIT**
  correspondre à un stade, un statut, une date, une personne ou un type de fichier.
- **A2.** Chaque niveau **DEVRAIT** compter entre 5 et 12 entrées. En deçà, le niveau est
  superflu ; au-delà, la sélection visuelle se dégrade — les travaux sur la capacité de
  la mémoire de travail (Miller, 1956 ; Cowan, 2001) situent le seuil d'aisance entre
  quatre et sept éléments simultanés.
- **A3.** La profondeur **NE DEVRAIT PAS** excéder cinq niveaux. Au-delà, le coût de
  navigation excède le gain de précision et la recherche plein texte devient supérieure.
- **A4.** Chaque niveau **DEVRAIT** porter un code court, stable et indépendant de son
  libellé. L'alternance de codes alphabétiques et numériques d'un niveau à l'autre
  (`AB` › `2` › `AC` › `4`) rend le niveau lisible dans le code lui-même. La méthode
  *Johnny.Decimal* et la Classification décimale universelle exploitent la même propriété.
- **A5.** Le libellé **PEUT** changer ; le code **NE DOIT PAS**. Les références externes
  pointent le code.
- **A6.** Aucune catégorie « Divers », « Autres » ou « À classer » **NE DOIT** figurer
  dans l'axe du Sujet. Le besoin qu'elles expriment est légitime, mais relève du sas (§ 14).

## 9. Axe B — STADE

### 9.1 Nature

L'axe du Stade répond à la question *où en est la production ?* Il est **cyclique,
ordonné et universel** : la même grille s'applique à tout projet, ce qui rend un dossier
lisible sans connaissance préalable de son domaine.

### 9.2 Grille canonique 0–9

Le référentiel retient une grille décimale : un stade de pilotage hors cycle (0), les
sept stades OBREDIM (1–7), un stade de rendement (8) et un stade de sort final (9).

| N° | Stade | Question | Produit épistémique | Livrables typiques |
|---|---|---|---|---|
| **0** | **PILOTAGE** | Où va l'ensemble ? | La **décision** de second ordre | Registre, jalons, arbitrages, comptes rendus |
| **1** | **OBSERVATION** | Qu'est-ce qui existe déjà ? | Le **donné** | Veille, audits, état de l'art, relevés, entretiens |
| **2** | **BORDURES** | Où s'arrête le système, par où échange-t-il ? | Le **système** | Périmètre, interfaces, conformité, exclusions |
| **3** | **RESSOURCES** | Avec quoi ? | Le **possible** | Inventaire des moyens, compétences, dotations, dépendances |
| **4** | **ÉVALUATION** | Qu'est-ce qui tient ? | La **décision** | Hypothèses testées, scénarios, arbitrages, décisions d'engagement |
| **5** | **CONCEPTION** | À quoi cela ressemble ? | La **forme** | Spécifications, plans, maquettes, modèles, chartes |
| **6** | **INSTALLATION** | On construit. | Le **fait** | Réalisations, configurations, contenus livrés, mises en service |
| **7** | **MAINTENANCE** | Cela tient-il ? | La **durée** | Procédures d'exploitation, incidents, supervision, correctifs |
| **8** | **RÉCOLTE** | Qu'est-ce que cela rend ? | Le **rendement** | Diffusion, acquisition, usage, résultats, mesure de la valeur |
| **9** | **DISPOSITION** | Quel sort final ? | La **clôture** | Versions closes, chantiers gelés, documents périmés |

### 9.3 Justification des deux extensions

**Le stade 8 (Récolte).** OBREDIM, conçu pour l'aménagement d'un terrain, ne thématise
pas le rendement : la parcelle produit d'elle-même. Aucun projet finalisé ne jouit de
cette gratuité. Le stade 8 comble ce manque en réservant une position à ce que le système
installé produit effectivement — usage, diffusion, revenus, autorité, effets mesurés.
Son omission est la cause ordinaire des projets techniquement achevés et pratiquement
sans effet.

**Le stade 9 (Disposition).** Ce stade constitue l'unique point de contact autorisé entre
l'axe du Stade et l'axe du Statut. Il ne s'agit pas d'une entorse au principe
d'orthogonalité : la *disposition* est, dans la doctrine archivistique (ISO 15489-1:2016),
une opération à part entière du cycle de vie — décider du sort final, appliquer une durée
de conservation, éliminer ou verser. Le stade 9 désigne cette opération, non l'état
« archivé » qui en résulte et qui, lui, demeure porté par le registre.

### 9.4 Règles

- **B1.** Le chiffre de stade **DOIT** avoir la même signification dans tous les projets.
- **B2.** Le stade **NE DOIT PAS** créer de répertoire au sein de l'axe du Sujet ; il
  **PEUT** en revanche organiser l'intérieur d'un dossier de projet, ce dossier constituant
  la feuille terminale de l'arbre des sujets.
- **B3.** L'ordre est **logique et non chronologique**. Un artefact de stade 1 peut être
  produit après un artefact de stade 6 ; sa position dans la grille exprime sa fonction,
  non sa date.
- **B4.** Tout artefact classé **DOIT** porter exactement un stade.

### 9.5 Gradient d'irréversibilité

Le coût de correction d'une erreur croît de manière monotone le long de la séquence 1→7 :
une erreur d'observation se corrige en retournant regarder ; une erreur d'installation se
paie indéfiniment en maintenance. La courbe empirique établie pour le logiciel (Boehm,
1981) exprime la même loi. Il en découle un **principe d'allocation d'effort** : investir
en amont dans la proportion inverse du coût de correction en aval.

## 10. Axe C — STATUT

### 10.1 Nature

L'axe du Statut répond à la question *qu'en fait-on maintenant ?* Il est **volatil,
exclusif et non hiérarchique**. Il **NE DOIT PAS** être matérialisé par des répertoires.

### 10.2 États

| État | Définition | Attente légitime | Régime d'attention |
|---|---|---|---|
| **INTENTION** | Formulé, non engagé, non doté | Aucune | Revue périodique |
| **ACTIF** | Engagé, doté, en progression sur les stades 1→6 | Avancement mesurable | Suivi continu |
| **SUSPENDU** | Engagé puis interrompu, avec condition de reprise explicite | Aucune, jusqu'à la condition | Revue périodique |
| **DOMAINE** | Installé, stabilisé, en régime de stade 7–8 | Constance, non progression | Supervision |
| **RESSOURCE** | Objet de connaissance mobilisable, sans échéance | Aucune | Aucune |
| **ARCHIVÉ** | Clos, conservé, sans usage courant prévu | Aucune | Aucune |

### 10.3 Machine à états

```
                    ┌──────────────┐
                    │  INTENTION   │
                    └──────┬───────┘
                     engagement (passage du stade 4)
                           │
                    ┌──────▼───────┐   interruption   ┌───────────┐
                    │    ACTIF     │◄────────────────►│ SUSPENDU  │
                    └──────┬───────┘    reprise       └─────┬─────┘
                           │                                │
              ┌────────────┴────────────┐                   │ péremption
              │                         │                   │
      mise en service            abandon / achèvement       │
      avec exploitation          sans exploitation          │
              │                         │                   │
       ┌──────▼───────┐          ┌──────▼───────┐◄──────────┘
       │   DOMAINE    │─────────►│   ARCHIVÉ    │
       └──────────────┘  fin de  └──────────────┘
                        l'exploitation

       ┌──────────────┐
       │  RESSOURCE   │  transversal : alimente les stades 1 et 3
       └──────────────┘  de tout projet, sans cycle propre
```

### 10.4 Règles

- **C1.** Tout objet piloté **DOIT** porter exactement un statut, inscrit au registre.
- **C2.** **Règle de sortie unique.** Un projet quittant l'état ACTIF **DOIT** entrer
  soit en DOMAINE — il est exploité, donc doté d'un régime de maintenance —, soit en
  ARCHIVÉ. **Aucune troisième issue n'est admise.** L'absence de cette règle est la cause
  principale de l'engorgement des systèmes de gestion de projet : les projets n'y meurent
  pas, ils cessent d'être mentionnés.
- **C3.** Le passage en DOMAINE **DOIT** s'accompagner de la production d'une procédure
  d'exploitation. Un domaine sans procédure est un projet inachevé qui se présente comme
  achevé.
- **C4.** Le passage en SUSPENDU **DOIT** s'accompagner de l'énoncé d'une condition de
  reprise vérifiable et d'une date de réexamen. À défaut de reprise à cette date, l'objet
  passe en ARCHIVÉ.
- **C5.** Un changement de statut **DOIT** être daté et motivé en une ligne. Cette trace
  constitue, à elle seule, l'historique décisionnel du portefeuille.

## 11. Composition : la coordonnée

Tout artefact est identifié par le triplet **(taxon, stade, statut)**.

```
  AXE SUJET  ──────►  où l'artefact réside      (répertoire)
  AXE STADE  ──────►  ce que l'artefact fait    (chiffre dans le nom)
  AXE STATUT ──────►  ce qu'on en attend        (valeur au registre)
```

Cette composition restitue en trois dimensions ce qu'une arborescence seule tentait
d'exprimer en une, sans multiplication combinatoire : *n* sujets, 10 stades et 6 statuts
décrivent *n × 60* situations avec *n* répertoires seulement.

---

# PARTIE IV — RÈGLES NORMATIVES

## 12. Les dix invariants

| N° | Invariant | Portée |
|---|---|---|
| **N1** | Un seul axe fait répertoire : le sujet. | DOIT |
| **N2** | Le chiffre de stade a la même signification partout. | DOIT |
| **N3** | Le statut vit au registre, jamais dans l'arborescence. | DOIT |
| **N4** | Tout artefact a une résidence unique. La duplication est interdite ; on référence. | DOIT |
| **N5** | Sortie unique : tout projet clos devient un domaine ou une archive. | DOIT |
| **N6** | Rien ne se supprime : on dispose (stade 9), on n'efface pas. | DEVRAIT |
| **N7** | Une ressource ne monte d'un niveau qu'au second usage avéré. | DEVRAIT |
| **N8** | Le sas se vide selon une périodicité fixe et courte. | DOIT |
| **N9** | Toute exception à une règle est écrite et datée dans le dossier de stade 0. | DOIT |
| **N10** | Le référentiel se révise à date fixe, jamais au fil de l'eau. | DEVRAIT |

**Commentaire sur N7 — la règle du second usage.** Le réflexe de « factoriser » un
document commun dès sa création produit des bibliothèques transverses volumineuses et
peu consultées. La règle inverse le fardeau de la preuve : un artefact demeure local à
son projet tant qu'un second projet ne l'a pas effectivement invoqué. La transversalité
se constate, elle ne s'anticipe pas.

**Commentaire sur N10.** Une classification est une infrastructure : sa valeur tient à sa
stabilité, non à son optimalité. Un référentiel révisé continûment n'est plus une
référence. Les révisions **DEVRAIENT** être groupées, versionnées et annoncées.

## 13. Nommage

### 13.1 Gabarit

```
AAAA-MM-JJ_S_objet-en-minuscules_vX.Y.Z.ext
│          │ │                   │
│          │ │                   └── version, facultative (SemVer)
│          │ └────────────────────── désignation, kebab-case, sans diacritiques
│          └──────────────────────── chiffre de stade (0–9)
└─────────────────────────────────── date au format ISO 8601
```

Exemples génériques :

```
2026-03-04_1_etude-de-marche-segment-b.md
2026-05-19_4_note-decision-go-nogo.md
2026-06-02_5_specification-fonctionnelle_v2.1.0.md
2026-07-11_7_incident-interruption-service.md
2026-09-30_0_revue-de-jalon-t3.md
```

### 13.2 Règles

- **D1.** La date **DOIT** suivre ISO 8601-1:2019, forme étendue `AAAA-MM-JJ`. Ce format
  est le seul dont l'ordre lexicographique coïncide avec l'ordre chronologique : le tri
  alphabétique par défaut produit un classement temporel correct, sans outil.
- **D2.** Les noms **NE DOIVENT PAS** comporter d'espaces, de diacritiques ni de
  caractères réservés. Le jeu recommandé se limite à `A–Z a–z 0–9 . _ -`, conformément
  aux ensembles portables des systèmes de fichiers et aux recommandations de préservation
  numérique. Les diacritiques compromettent la portabilité par variation de normalisation
  Unicode (NFC/NFD).
- **D3.** Le versionnage, lorsqu'il s'applique à un artefact évolutif, **DEVRAIT** suivre
  le versionnage sémantique (`MAJEUR.MINEUR.CORRECTIF`) : incrément majeur en cas de
  rupture de compatibilité ou de changement de périmètre, mineur en cas d'ajout,
  correctif en cas de correction sans effet fonctionnel.
- **D4.** La désignation **DEVRAIT** être intelligible hors contexte. Un nom qui n'a de
  sens que dans son répertoire perd toute valeur dès la première extraction.

## 14. Le sas

### 14.1 Fondement

Aucune classification ne classe sans reste (§ 6.2). Le sas est le dispositif qui
**absorbe l'indéterminé sans le laisser polluer la taxonomie**. Son absence produit soit
des catégories « Divers » dans l'axe du Sujet — proscrites par A6 —, soit un
contournement pur et simple du système.

### 14.2 Règles

- **E1.** Le sas **DOIT** être distinct de l'arborescence des sujets, et identifié comme
  zone de flux et non de stock.
- **E2.** Le sas **DOIT** être vidé selon une périodicité fixe, **DEVRAIT** être
  hebdomadaire, et **NE DOIT PAS** excéder le mois.
- **E3.** Un artefact séjournant dans le sas au-delà de deux cycles de purge **DOIT**
  être traité comme le signal d'une décision non prise. Il relève alors d'un arbitrage de
  stade 4 et non d'un problème de rangement.
- **E4.** Le volume du sas **DEVRAIT** être suivi comme un indicateur (§ 17). Une
  croissance monotone indique une défaillance du système, non de l'utilisateur.

## 15. Bouclage et apprentissage

Le stade 7 (Maintenance) n'est pas terminal : il constitue l'organe de régulation du
cycle. Ce qu'il observe ne renvoie pas toujours au même point, et la qualité du pilotage
se mesure à la justesse du point de retour.

| Ce que révèle la maintenance | Retour vers | Nature de l'apprentissage |
|---|---|---|
| Un écart ponctuel à la norme | **6** — on répare | Boucle simple |
| Une conception inadéquate | **5** — on redessine | Boucle simple étendue |
| Des bordures mal tracées | **2** — on reconstitue l'objet | Boucle double (Argyris & Schön, 1978) |
| Une observation initiale fausse | **1** — on recommence | Réamorçage |

- **F1.** La récurrence d'incidents de même famille **DOIT** déclencher un examen du
  point de retour. Réparer en boucle simple ce qui relève de la boucle double est
  l'erreur de pilotage la plus fréquente et la plus coûteuse.
- **F2.** Le dispositif de maintenance **DEVRAIT** posséder une variété au moins égale à
  celle du système installé — application directe de la loi de la variété requise
  (Ashby, 1956). Il s'ensuit que la maintenance **DOIT** être conçue au stade 5, en même
  temps que l'objet, et non improvisée après le stade 6.

---

# PARTIE V — MISE EN ŒUVRE

## 16. Niveaux de conformité

Le référentiel définit trois niveaux, afin qu'une adoption partielle demeure cohérente.

| Niveau | Exigences | Effort d'entrée |
|---|---|---|
| **1 — Minimal** | N1, N3, N4, D1. L'arborescence n'exprime que le sujet ; les dates sont normalisées ; aucun doublon. | Faible |
| **2 — Standard** | Niveau 1 + grille 0–9 (N2), registre des statuts avec règle de sortie unique (N5), sas régulé (E1–E3). | Moyen |
| **3 — Complet** | Niveau 2 + N6 à N10, gabarit de nommage complet (D1–D4), bouclage documenté (F1–F2), indicateurs (§ 17). | Élevé |

Une implémentation **DOIT** déclarer son niveau. Une implémentation qui déroge à une
exigence de son niveau déclaré **DOIT** documenter la dérogation (N9).

## 17. Indicateurs de santé

Les indicateurs suivants sont proposés à titre de recommandation. Ils mesurent le
**système de classification**, non la performance des projets.

| Indicateur | Définition | Signal d'alerte |
|---|---|---|
| **Charge du sas** | Nombre d'artefacts non classés | Croissance sur trois cycles consécutifs |
| **Latence de classement** | Délai médian entre création et classement | Supérieur à un cycle de purge |
| **Taux de sortie** | Projets clos / projets ouverts sur la période | Durablement inférieur à 1 |
| **Âge des actifs** | Âge médian des objets en statut ACTIF | Croissance continue : le portefeuille se fige |
| **Ratio 1–4 / 5–6** | Volume produit en amont rapporté à l'aval | Inférieur à 0,5 : amont insuffisant |
| **Domaines sans procédure** | Objets en DOMAINE dépourvus de procédure d'exploitation | Toute occurrence (violation de C3) |
| **Récurrence d'incidents** | Part des incidents de famille déjà rencontrée | Supérieure à 30 % : mauvais point de retour (F1) |
| **Profondeur moyenne** | Niveaux parcourus pour atteindre un artefact | Supérieure à 5 (violation de A3) |

## 18. Procédure d'adoption

### 18.1 Système neuf

1. Définir l'axe du Sujet — trois niveaux suffisent initialement ; la profondeur croîtra.
2. Instancier la grille 0–9 sur un projet unique, à titre d'étalon.
3. Ouvrir le registre des statuts et y porter l'existant.
4. Instituer le sas et sa périodicité de purge.
5. Déclarer le niveau de conformité visé.

### 18.2 Système existant

La migration d'un système en exploitation présente un coût réel — chemins rompus, liens
cassés, habitudes défaites — qui **DOIT** être évalué avant décision.

- **G1.** La migration **NE DEVRAIT PAS** être conduite au fil de l'eau, mais à une date
  de jalon, en un seul mouvement.
- **G2.** Une table de correspondance ancien → nouveau **DOIT** être produite avant tout
  déplacement, et conservée en stade 0.
- **G3.** Lorsque le coût de migration excède le bénéfice attendu, la **voie douce**
  **DEVRAIT** être retenue : appliquer le référentiel aux objets neufs, geler l'existant,
  et laisser l'attrition résoudre la dualité. Un système partiellement conforme et stable
  vaut mieux qu'une migration inachevée.
- **G4.** L'ancien système **NE DOIT PAS** être supprimé avant l'expiration d'une période
  d'observation d'au moins un cycle de purge complet.

## 19. Anti-modèles

| Anti-modèle | Manifestation | Règle violée |
|---|---|---|
| **Le répertoire d'humeur** | Dossiers « Urgent », « En cours », « Important » | N1, C1 |
| **L'arbre calendaire** | Un niveau par année ou par mois | A1 — la date est une métadonnée |
| **L'arbre nominatif** | Un niveau par personne | A1 — la personne est une facette, non un sujet |
| **Le fourre-tout** | Catégorie « Divers » installée durablement | A6, E1 |
| **La factorisation prématurée** | Bibliothèque transverse créée avant tout second usage | N7 |
| **Le projet zombie** | Objet ni actif, ni clos, ni archivé | N5, C2 |
| **Le domaine orphelin** | Objet exploité sans procédure d'exploitation | C3 |
| **La copie de sécurité** | Duplication manuelle « au cas où » | N4 |
| **La réforme perpétuelle** | Révision continue de la taxonomie | N10 |
| **Le stade escamoté** | Passage direct de l'idée à la réalisation | Voir § 20 |

## 20. Pathologies par omission de stade

Chaque stade escamoté produit une défaillance caractéristique. Cette lecture négative
constitue un instrument de diagnostic autonome.

| Stade omis | Pathologie | Signe clinique |
|---|---|---|
| **1 Observation** | Solutionnisme | La solution précède le diagnostic ; le projet s'impose au milieu au lieu de s'y insérer |
| **2 Bordures** | Dilatation | Périmètre indéfini, dérive du contenu, responsabilités enchevêtrées, externalités ignorées |
| **3 Ressources** | Le beau plan | Conception irréprochable et non finançable ; impossibilité découverte tardivement |
| **4 Évaluation** | Engagement irréversible | Aucun moment institué où le projet peut mourir ; les coûts irrécupérables décident |
| **5 Conception** | Improvisation | Aucune représentation partagée ; le projet n'existe que dans une seule tête |
| **6 Installation** | Paralysie analytique | Planification perpétuelle ; le réel n'est jamais touché, donc jamais démenti |
| **7 Maintenance** | Entropie | L'objet livré se dégrade ; le succès de la livraison masque l'échec de la durée |
| **8 Récolte** | Production sans effet | L'objet fonctionne et ne sert à personne ; aucune mesure de l'usage |
| **9 Disposition** | Sédimentation | Le système accumule sans jamais clore ; la recherche se dégrade avec le volume |

## 21. Conditions de validité et limites

### 21.1 Le référentiel est pertinent lorsque

1. le substrat **préexiste** et ne peut être remis à zéro ;
2. les erreurs se manifestent **lentement**, après la mise en service ;
3. le coût cumulé d'exploitation **domine** le coût de construction ;
4. le portefeuille compte **plusieurs objets simultanés** de nature hétérogène ;
5. l'horizon de conservation excède la durée d'un projet.

### 21.2 Le référentiel est mal adapté lorsque

1. l'objet n'existe pas encore et **rien ne peut être observé** : l'expérimentation
   rapide est alors supérieure à l'analyse préalable ;
2. l'environnement varie **plus vite que le cycle** ne se boucle : l'observation est
   périmée avant la conception ;
3. la situation est **chaotique** au sens de Cynefin (Snowden & Boone, 2007) : il faut
   agir pour stabiliser, comprendre ensuite ;
4. le coût de l'essai est **négligeable** : mieux vaut tester qu'arbitrer ;
5. le volume est **trivial** : en deçà d'une centaine d'artefacts, le coût du référentiel
   excède son bénéfice.

### 21.3 Limites intrinsèques

Quatre réserves, qui sont des propriétés du modèle et non des défauts d'application.

**Biais conservateur.** Partir de l'existant incline à le prolonger. Le modèle excelle à
insérer, mal à rompre : une innovation de rupture est par construction ce qui ne se déduit
pas de l'observation du milieu.

**Coût d'entrée.** Quatre stades de lecture avant toute production visible : exigence
difficile à tenir lorsque le financement dépend de livrables précoces.

**Frontière poreuse entre les stades 4 et 5.** Évaluer suppose de se représenter ce que
l'on évalue ; on conçoit donc en évaluant. La séquence est logique, non chronologique
(B3) — l'oublier produit un formalisme stérile.

**Postulat d'observabilité.** Le modèle suppose que le réel se laisse relever. Dans les
systèmes sociaux, l'observation modifie l'observé et les acteurs ont intérêt à ce qui est
relevé ; le stade 1 y devient lui-même un enjeu politique. Cette dimension, que la
méthodologie des systèmes souples thématise explicitement, demeure un angle mort du
présent référentiel.

## 22. Gouvernance du référentiel

- **H1.** Le référentiel **DOIT** être versionné et daté.
- **H2.** Toute modification **DOIT** être accompagnée d'une note d'évolution indiquant
  la règle touchée et la raison.
- **H3.** Les révisions **DEVRAIENT** être groupées à date fixe (N10).
- **H4.** Une règle abrogée **NE DOIT PAS** être supprimée du document : elle est marquée
  comme obsolète, avec sa date et son motif d'abrogation. La cohérence des systèmes
  déployés antérieurement en dépend.

---

# ANNEXES

## Annexe A — Formulation condensée

> Un projet consiste à inscrire une forme dans un milieu qui lui préexiste et lui
> survivra. Trois questions indépendantes se posent à son propos : **de quoi s'agit-il**,
> **où en est-on**, **qu'en attend-on**. Un seul dispositif — l'arborescence — ne peut y
> répondre sans se dégrader. On les sépare donc : le sujet fait l'arbre, le stade fait le
> chiffre, le statut fait le registre. Le cycle n'est pas une flèche mais une spirale :
> la maintenance réalimente l'observation, et la clôture d'un projet n'a que deux issues
> — devenir un domaine, ou devenir une archive.

## Annexe B — Aide-mémoire de la grille 0–9

```
0  PILOTAGE      où va l'ensemble          registre, jalons, arbitrages
1  OBSERVATION   ce qui existe déjà        veille, audits, relevés
2  BORDURES      où cela s'arrête          périmètre, interfaces, conformité
3  RESSOURCES    avec quoi                 moyens, compétences, dépendances
4  ÉVALUATION    ce qui tient              scénarios, décisions d'engagement
5  CONCEPTION    à quoi cela ressemble     spécifications, plans, modèles
6  INSTALLATION  on construit              réalisations, mises en service
7  MAINTENANCE   cela tient-il             exploitation, incidents, supervision
8  RÉCOLTE       ce que cela rend          diffusion, usage, résultats
9  DISPOSITION   quel sort final           clôture, conservation, versement
```

## Annexe C — Table de correspondance des vocabulaires

| Référentiel | OBREDIM | PARA | PDCA | Cycle de vie documentaire |
|---|---|---|---|---|
| Stade 0 | — | — | *Act* | — |
| Stades 1–4 | O, B, R, E | Resources | *Plan* | Création |
| Stades 5–6 | D, I | Projects | *Do* | Courant |
| Stade 7 | M | Areas | *Check* | Courant |
| Stade 8 | — | Areas | *Check* | Courant |
| Stade 9 | — | Archives | — | Intermédiaire, puis définitif |

## Annexe D — Bibliographie

**Classification et catégorisation**

- Ranganathan, S. R., *Colon Classification*, Madras Library Association, 1933.
- Ranganathan, S. R., *Prolegomena to Library Classification*, 1937 (3ᵉ éd. 1967).
- Vickery, B. C., *Faceted Classification: A Guide to Construction and Use of Special Schemes*, Aslib, 1960.
- Rosch, E., « Principles of Categorization », in *Cognition and Categorization*, Erlbaum, 1978.
- Lakoff, G., *Women, Fire, and Dangerous Things*, University of Chicago Press, 1987.
- Bowker, G. C. & Star, S. L., *Sorting Things Out: Classification and Its Consequences*, MIT Press, 1999.
- Weinberger, D., *Everything Is Miscellaneous: The Power of the New Digital Disorder*, Times Books, 2007.

**Gestion documentaire et archivistique**

- ISO 15489-1:2016, *Information et documentation — Gestion des documents d'activité*.
- ISO 14721:2012, *Systems and software engineering — Open Archival Information System (OAIS)*.
- ISO 8601-1:2019, *Éléments de données et formats d'échange — Représentation des dates et des heures*.
- Upward, F., « Structuring the Records Continuum », *Archives and Manuscripts*, 1996.
- Digital Preservation Coalition, *Digital Preservation Handbook*, 2ᵉ éd.

**Cycle de projet et conception**

- Mollison, B., *Permaculture: A Designers' Manual*, Tagari, 1988.
- Holmgren, D., *Permaculture: Principles and Pathways Beyond Sustainability*, Holmgren Design Services, 2002.
- Checkland, P., *Systems Thinking, Systems Practice*, Wiley, 1981.
- Simon, H. A., *The Sciences of the Artificial*, MIT Press, 1969.
- Sarasvathy, S. D., « Causation and Effectuation », *Academy of Management Review*, 26(2), 2001.
- Boehm, B., *Software Engineering Economics*, Prentice Hall, 1981.
- Snowden, D. & Boone, M., « A Leader's Framework for Decision Making », *Harvard Business Review*, nov. 2007.

**Systèmes, régulation, apprentissage**

- von Bertalanffy, L., *General System Theory*, Braziller, 1968.
- Ashby, W. R., *An Introduction to Cybernetics*, Chapman & Hall, 1956.
- Argyris, C. & Schön, D., *Organizational Learning: A Theory of Action Perspective*, Addison-Wesley, 1978.
- Luhmann, N., *Soziale Systeme*, Suhrkamp, 1984.

**Organisation personnelle et méthode**

- Allen, D., *Getting Things Done*, Viking, 2001.
- Forte, T., *Building a Second Brain*, Atria Books, 2022.
- Ahrens, S., *How to Take Smart Notes*, 2017.

**Génie logiciel et conventions**

- Parnas, D. L., « On the Criteria To Be Used in Decomposing Systems into Modules », *CACM*, 15(12), 1972.
- Dijkstra, E. W., « On the role of scientific thought », EWD447, 1974.
- Bradner, S., *RFC 2119 — Key words for use in RFCs to Indicate Requirement Levels*, IETF, 1997.
- Preston-Werner, T., *Semantic Versioning 2.0.0*.

**Capacité cognitive**

- Miller, G. A., « The Magical Number Seven, Plus or Minus Two », *Psychological Review*, 63(2), 1956.
- Cowan, N., « The magical number 4 in short-term memory », *Behavioral and Brain Sciences*, 24(1), 2001.

---

*Fin du référentiel — version 1.0.*
