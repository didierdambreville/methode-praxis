# Gabarit de nommage et de classification

*Aide-mémoire du geste ④. Règles complètes : méthode PRAXIS §4.4 et annexe A ; référentiel RCUP §13.*

## Le gabarit

```
AAAA-MM-JJ_S_designation-en-kebab-case_vX.Y.Z.ext
│          │ │                          │
│          │ │                          └─ version SemVer — artefacts évolutifs seulement
│          │ └─ désignation intelligible hors contexte
│          └─ chiffre de stade (0–9)
└─ date ISO 8601 — le tri alphabétique EST le tri chronologique
```

**Jeu de caractères autorisé :** `A–Z a–z 0–9 . _ -` — sans espaces, sans diacritiques (é → e, à → a…).

## La grille des stades

| N° | Stade | Question | Livrables typiques |
|---|---|---|---|
| **0** | PILOTAGE | où va l'ensemble ? | registre, jalons, revues, arbitrages, comptes rendus |
| **1** | OBSERVATION | qu'est-ce qui existe déjà ? | veille, audits, état de l'art, relevés, entretiens |
| **2** | BORDURES | où cela s'arrête-t-il ? | périmètre, interfaces, conformité, exclusions |
| **3** | RESSOURCES | avec quoi ? | inventaires de moyens, compétences, dotations, dépendances |
| **4** | ÉVALUATION | qu'est-ce qui tient ? | hypothèses testées, scénarios, décisions d'engagement |
| **5** | CONCEPTION | à quoi cela ressemble ? | spécifications, plans, maquettes, modèles, chartes |
| **6** | INSTALLATION | on construit | réalisations, configurations, mises en service |
| **7** | MAINTENANCE | cela tient-il ? | procédures d'exploitation, incidents, correctifs |
| **8** | RÉCOLTE | qu'est-ce que cela rend ? | diffusion, usage, résultats, mesure de la valeur |
| **9** | DISPOSITION | quel sort final ? | versions closes, chantiers gelés, documents périmés |

L'ordre est **logique, non chronologique** : un artefact de stade 1 peut être produit après un artefact de stade 6 ; le chiffre exprime sa fonction, pas sa date.

## Exemples

```
2026-08-24_1_etude-marche-segment-pme.md
2026-08-30_2_perimetre-conformite-rgpd.md
2026-09-02_4_note-decision-go-nogo.md
2026-09-15_5_specification-fonctionnelle_v1.2.0.md
2026-10-07_6_configuration-boutique-en-ligne.md
2026-11-12_7_incident-interruption-service.md
2027-01-10_0_revue-jalon-t1.md
2027-03-01_8_mesure-benefices-6-mois.md
2027-06-30_9_cloture-version-1.md
```

## Les cinq règles qui accompagnent le nom

1. **Résidence unique** — un fichier vit à un seul endroit ; ailleurs, on le référence, on ne le copie pas.
2. **Le répertoire n'exprime que le sujet** — jamais de dossier de stade, de statut, de date ou de personne.
3. **Le statut vit au registre** (tableau de bord), jamais dans le nom ni dans l'arborescence.
4. **Rien ne se supprime** — un artefact périmé passe au stade 9 ; on dispose, on n'efface pas.
5. **Second usage** — un fichier ne monte en `R-RESSOURCES/` que lorsqu'un second projet l'a effectivement invoqué.
