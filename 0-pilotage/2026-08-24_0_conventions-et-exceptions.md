# Conventions de classement du dépôt et exceptions déclarées

*Artefact de stade 0 (pilotage) du dépôt `methode-praxis`. Tenu au titre de l'invariant **N9** du RCUP : toute exception à une règle est écrite et datée dans le dossier de stade 0.*

## Déclaration de conformité

Le présent dépôt applique à lui-même le Référentiel de classification unifiée des projets (RCUP v1.0), au **niveau 3 (complet)** :

- l'arborescence n'exprime que des positions de production — les répertoires `0-pilotage/`, `3-ressources/`, `5-conception/` et `7-exploitation/` organisent l'**intérieur** du dossier de projet par stade, comme l'autorise la règle **B2** (le dépôt entier est la feuille terminale d'un axe de sujets qui, lui, vit chez chaque utilisateur) ;
- chaque artefact porte le gabarit de nommage **D1–D4** : `AAAA-MM-JJ_S_designation_vX.Y.Z.ext` ;
- les documents fondateurs conservent leur **date de publication propre** (2026-08-18) et leur numéro de version d'origine (TELOS 1.1 → `v1.1.0`, SOBRE 1.1 → `v1.1.0`), conformément à D3.

## Attribution des stades (motifs)

| Artefacts | Stade | Motif |
|---|---|---|
| Ce document | 0 — pilotage | conventions et exceptions du dépôt lui-même |
| Corpus fondateur (RCUP, TELOS, SOBRE) et ses licences | 3 — ressources | moyens de connaissance mobilisés par la conception de PRAXIS ; en portefeuille utilisateur, ces objets relèvent du statut RESSOURCE |
| Méthode, tableau de bord, gabarits, modèles | 5 — conception | modèles, chartes et spécifications : la forme de la méthode |
| Notice d'utilisation, exemple d'arborescence | 7 — exploitation | procédures et aides d'exploitation de la méthode installée |

## Exceptions déclarées (N9)

| Date | Exception | Règle concernée | Motif |
|---|---|---|---|
| 2026-09-01 | Le fichier SOBRE, publié le 2026-08-24 sous le nom `..._v1.0.0`, est renommé `..._v1.1.0` sans changer de contenu | D3 (numéro de version) | erreur de nommage à la publication initiale : le PDF versé porte « Version 1.1 · 18 août 2026 » sur sa page de titre, et le site sert ce même fichier comme v1.1 ; seul l'en-tête du Markdown était resté à 1.0, il est corrigé. Les renvois de la méthode PRAXIS à « SOBRE v1.0 » sont rectifiés en conséquence |
| 2026-08-24 | `README.md` et `LICENSE` conservent leur nom et leur position à la racine, sans date ni stade | D1 (gabarit de nommage) | conventions de la plateforme GitHub : ces deux noms sont détectés et affichés par l'hébergeur ; les renommer romprait l'affichage de la page d'accueil et la reconnaissance de la licence |
| 2026-08-24 | Les fichiers de ce dépôt existent en une copie par clone, ainsi que dans l'archive de distribution | N4 (résidence unique) | il s'agit de copies de **distribution** d'une même version publiée, non de doublons de travail ; la source unique de vérité est le dépôt Git |

## Correspondance avec les noms d'usage

Dans la doctrine (méthode, notice), les artefacts sont cités par leur **nom d'usage** dans le portefeuille de l'utilisateur — `tableau_de_bord.html`, `[NOM]_Contexte_Projet.md`, `[NOM]_Pilotage.xlsx` — car c'est sous ces noms de travail qu'ils vivent une fois copiés chez l'utilisateur. La table du README donne la correspondance nom d'usage → artefact du dépôt.
