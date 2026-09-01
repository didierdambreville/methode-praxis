# Méthode PRAXIS

**Méthode de travail entrepreneuriale — classer, piloter, collaborer avec l'assistant IA.**

Version 1.2 · 1er septembre 2026 · Auteur : D. Dambreville · **Domaine public (CC0 1.0)**

---

PRAXIS est une méthode opératoire pour entrepreneurs (solo ou petite équipe) conduisant plusieurs projets à la fois. Elle unifie en un seul système de travail :

- le **Référentiel de classification unifiée des projets** (RCUP) — *où ranger, et dans quel état est chaque chose* : trois axes orthogonaux (sujet × stade × statut), un sas d'entrée, un gabarit de nommage ;
- la **méthode TELOS** — *comment conduire un projet pour qu'il produise un bénéfice vérifié* : énoncé de bénéfice, critères d'abandon, diagnostic de contingence, flux limité, indicateurs contradictoires ;
- la **méthode SOBRE** — *comment instruire un assistant IA pour qu'il travaille juste* : sobriété, orthogonalité, frontière d'instruction, vérification humaine ;
- les pratiques de flux de la méthode **Kanban**, reprises par soustraction — *où le travail est arrêté, et depuis quand* : sept colonnes adossées à la grille des stades, une limite d'encours affichée par colonne, des règles de sortie explicites ;
- deux **gabarits opératoires** : le document de contexte de projet et le classeur de pilotage ;
- un **tableau de bord HTML autonome** : registre des projets, tableau de flux, neuf indicateurs à seuils, journal des décisions, suivi du sas — sans serveur, sans dépendance, hors ligne.

## L'usage minimaliste

```
① DÉPOSER         tout fichier entrant va dans le sas, sans réfléchir
② FAIRE ANALYSER  l'assistant IA propose classement, données extraites, mises à jour
③ VÉRIFIER        l'humain contrôle chaque donnée contre la source
④ CLASSER         renommage au gabarit  AAAA-MM-JJ_S_designation_vX.Y.Z.ext
⑤ METTRE À JOUR   contexte de projet · classeur de pilotage · tableau de bord
```

Une seule réunion obligatoire : la **revue hebdomadaire** (30–60 min), qui exécute les gestes ② à ⑤ et lit le tableau de flux **de droite à gauche** : aider à finir avant de commencer.

## Nouveau en 1.2 — le tableau de flux

```
  SAS  │ INTENTION │ INSTRUCTION │ EN COURS  │ VÉRIFICATION │ RÉCOLTE │ SORTI
       │  st. 0–1  │   st. 2–4   │  st. 5–6  │    st. 7     │  st. 8  │ st. 9
       │     —     │  limite 3   │ limite 2  │   limite 2   │    —    │   —
                                  / personne
```

La colonne d'un objet se **déduit** de son statut et de son stade : aucun champ nouveau, aucune saisie nouvelle, aucune réunion nouvelle. Le tableau affiche l'occupation de chaque colonne face à sa limite et l'âge de chaque carte ; il en dérive le **temps de cycle** (médiane et 85ᵉ centile) et le **débit**, qui alimentent les indicateurs 3, 4 et 5 sans agrandir le panier. Le détail est au chapitre 6 de la méthode, les réglages à l'annexe F.

## Commencer

1. Lire la **[notice d'utilisation](7-exploitation/2026-09-01_7_notice-utilisation_v1.1.0.md)** — installation en 15 minutes.
2. Ouvrir **[le tableau de bord](5-conception/2026-09-01_5_tableau-de-bord-praxis_v1.2.0.html)** dans un navigateur (télécharger le fichier, double-cliquer, puis l'enregistrer sous son nom d'usage `tableau_de_bord.html`).
3. Lire la **[méthode intégrale](5-conception/2026-09-01_5_methode-praxis_v1.2.0.md)** ([PDF](5-conception/2026-09-01_5_methode-praxis_v1.2.0.pdf)) pour la doctrine, les règles et les annexes.

## Contenu du dépôt

Le dépôt s'applique à lui-même le référentiel de classification qu'il publie : les répertoires portent le **stade** de production (grille 0–9 du RCUP) et chaque artefact le gabarit `AAAA-MM-JJ_S_designation_vX.Y.Z.ext`. Les conventions et exceptions sont déclarées dans [`0-pilotage/`](0-pilotage/2026-08-24_0_conventions-et-exceptions.md).

| Répertoire (stade) | Artefact | Rôle |
|---|---|---|
| [`0-pilotage/`](0-pilotage/) | conventions-et-exceptions | Déclaration de conformité RCUP du dépôt (N9) |
| [`3-ressources/`](3-ressources/) | referentiel-classification-unifiee (md + pdf) | Document fondateur : le RCUP intégral |
| | methode-telos-edition-publique (md + pdf) | Document fondateur : la méthode TELOS intégrale |
| | methode-sobre-architecture-instruction-llm (md + pdf) | Document fondateur : la méthode SOBRE intégrale |
| | licences-du-corpus | Licences propres des documents fondateurs |
| [`5-conception/`](5-conception/) | **methode-praxis** (md + pdf) | **La méthode intégrale** |
| | tableau-de-bord-praxis (html) | Le tableau de bord autonome — registre, **tableau de flux**, indicateurs (nom d'usage : `tableau_de_bord.html`) |
| | gabarit-nommage-classification | Aide-mémoire du nommage et des stades |
| | gabarit-prompt-analyse-sas | Prompt canonique du geste ② |
| | gabarit-instructions-projet | Instructions à coller dans l'espace de projet de l'assistant |
| | modele-contexte-projet (md) | Modèle de mémoire de projet (nom d'usage : `[NOM]_Contexte_Projet.md`) |
| | modele-pilotage-projet (xlsx) | Modèle de classeur de pilotage (nom d'usage : `[NOM]_Pilotage.xlsx`) |
| [`7-exploitation/`](7-exploitation/) | notice-utilisation | **La notice pas à pas** |
| | exemple-arborescence | Une arborescence de portefeuille commentée |

## Licences

La méthode PRAXIS, sa notice, ses gabarits propres et son tableau de bord sont versés au **domaine public** ([CC0 1.0](LICENSE)) : copiez, modifiez, redistribuez, sans condition.

Les pratiques Kanban dont le tableau de flux est dérivé relèvent du domaine public de la pratique professionnelle : elles ne sont pas un document du corpus et n'emportent aucune obligation de licence.

Les documents fondateurs inclus dans [`3-ressources/`](3-ressources/) demeurent sous leurs licences propres (CC BY 4.0 / CC BY-SA 4.0 — voir [licences du corpus](3-ressources/2026-08-24_3_licences-du-corpus.md)).
