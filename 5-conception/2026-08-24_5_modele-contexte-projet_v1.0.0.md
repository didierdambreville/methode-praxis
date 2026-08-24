# [NOM DU PROJET] — Contexte de Projet
*Document de référence pour le Projet « [NOM DU PROJET] ». À jour du [JJ/MM/AAAA]. À rafraîchir après chaque changement structurant (voir §10).*

> **Mode d'emploi de ce gabarit** : remplacez tous les éléments entre [crochets], supprimez les sections sans objet, et effacez les lignes de guidage en italique commençant par « ℹ️ » une fois la section rédigée. Règle d'or : ce document est la *mémoire distillée* du projet — court, exact, à jour. Tout ce qui n'a plus cours part en Chronologie (§6).

---

## 1. Identité & mission

*ℹ️ Qui porte le projet, ce qu'il produit, pour qui, à quel prix. Cinq lignes suffisent si elles sont précises.*

- **Structure porteuse** : [raison sociale, forme juridique, pays]. [Profil de l'équipe : solo / N personnes ; compétences clés ; limites assumées — ex. « techniquement autonome mais non-développeur »].
- **Marques / entités du portefeuille** : [MARQUE 1 (domaine.fr — ce projet)], [MARQUE 2 (domaine.fr, activité)], [MARQUE 3 (…)].
- **[NOM DU PROJET]** : [définition en une phrase : nature de l'activité]. Signature / promesse : « [SLOGAN] ». Produit ou service central : **[NOM DU PRODUIT]**, [description : nature, fréquence, canal de livraison, horaire s'il y a lieu].
- **Cible** : [segments de clientèle]. Personas de référence : [Persona A (profil résumé)] et [Persona B (profil résumé)].
- **Offre** : [prix et modalité — ex. abonnement X €/mois, prestation forfaitaire, licence annuelle]. Lancement commercial : [date ou état].

## 2. Positionnement du produit / service

*ℹ️ Le format exact du livrable, ses sections ou composantes fixes, le ton, et surtout les règles non négociables (juridiques, éthiques, éditoriales). C'est la section qui empêche les dérives.*

- **Format** : [support, langue, ton, gabarit de référence et sa version — ex. template XYZ_V1.0].
- **Structure fixe** : [SECTION A] → [SECTION B] → [SECTION C] → [MENTION OBLIGATOIRE / AVERTISSEMENT — intangible].
- **Conformité ([cadre applicable : RGPD, réglementation sectorielle, CGV…])** : [ce qui est autorisé]. Interdits absolus : [liste explicite des formulations, contenus ou pratiques proscrits]. Documents de cadrage : [charte / CGV / politique — état : rédigé / en cours (tâche N du Gantt)].
- **Règles de rigueur** : [ex. toute donnée chiffrée sourcée et datée ; tout écart significatif vs la version précédente explicitement commenté ; les inconnues déclarées, jamais inventées].

## 3. Stack technique & outillage

*ℹ️ Un inventaire par fonction, pas par marque : chaque ligne dit à quoi sert l'outil. Notez les bugs connus et corrigés — ils resservent.*

- **Site & vente** : [CMS, e-commerce, prestataire de paiement, extensions clés — mentionner les bugs identifiés/corrigés], [outil de sauvegarde], [analytics].
- **Communication / e-mailing** : [plateforme — identifier les listes/segments : liste #N = production, liste #M = test].
- **Automatisation** : [outil, mode d'hébergement, version]. Workflows en service : [workflow 1 (rôle, version)], [workflow 2 (…)].
- **IA / APIs** : [fournisseur 1 (usage, modèle, depuis le JJ/MM)] ; [fournisseur 2 (usage, modèle)] ; [sources de données (coût, clé requise ou non)].
- **Environnement de travail** : [poste, logiciels, gestionnaire de mots de passe, stockage/synchronisation].
- **Marketing** : [canaux payants — compte, budget/jour, plafonds]. [Obligations de conformité associées — état, échéance, n° de tâche].

## 4. Architecture du processus central — v[X.Y.Z] (référence)

*ℹ️ Décrivez le pipeline de production étape par étape, dans l'ordre d'exécution, avec pour chaque étape : ce qu'elle fait, ses règles dures, ses garde-fous. Terminez par les principes d'ingénierie actés.*

Pipeline « [nom du pipeline : ex. collecte → vérification → assemblage] », [N] étapes/nœuds, déclenchement : [cron / manuel / événement].

1. **[Étape 1 — nom]** — [ce qu'elle produit, format de sortie, contraintes : budgets, plafonds, hiérarchie des sources].
2. **[Étape 2 — nom]** — [entrées, traitements, sorties ; ce qui constitue la « source de vérité »].
3. **[Étape 3 — nom]** — [règles imposées, interdictions].
4. **[Mémoire / persistance]** — [ce qui est stocké entre deux exécutions, où, durée de validité, mécanisme de secours si vide].
5. **[Assemblage / production du livrable]** — [N] règles dures : [liste des règles bloquantes].
6. **[Vérification déterministe (bloquante)]** — [contrôles automatiques : motifs interdits, sections obligatoires, plausibilité, comparaison avec la version précédente, cohérence avec la source de vérité — seuils chiffrés]. Échec → [procédure : alerte, non-livraison].
7. **[Relecture / contrôle qualité]** — [méthode, format du verdict, critères de blocage].
8. **[Livraison]** puis [archivage / stockage].

Principes d'ingénierie actés : [ex. les données dures viennent de sources de données, jamais d'un LLM ; le déterministe avant l'IA pour tout ce qui est vérifiable ; un livrable bloqué vaut mieux qu'un livrable faux ; distinguer anomalie réelle et événement exceptionnel légitime].

## 5. Économie & coûts (référentiel)

*ℹ️ Les coûts constatés, la cible, les tarifs unitaires des fournisseurs, et les règles budgétaires. C'est la section qui déclenche les alertes de dérive.*

- **Version en production** : coût constaté [X €/jour ou /mois], tendance [stable / en dérive — cause identifiée].
- **Version en préparation** : cible ≤ [Y €/jour ou /mois] ([décomposition par poste]). Tarifs unitaires : [fournisseur A = prix] ; [fournisseur B = prix].
- **Règles budgétaires actées** : [ex. tout débogage en mode économe (données épinglées / environnement de test) ; jamais d'appel sans plafond ; relevé de coût quotidien (tâche N)]. Incidents de coût passés : [date : montant — leçon retenue].
- Coût technique complet visé : **[X €/mois]**, soit [équivalence parlante — ex. moins de N clients].

## 6. Chronologie des décisions structurantes

*ℹ️ L'historique compressé : périodes, décisions, incidents et leçons. Chaque entrée en 1 à 3 lignes. C'est ici que migre ce qui n'est plus « courant ».*

- **[Période 1]** : [construction initiale ; jalons ; travaux stratégiques réalisés].
- **[Période 2]** : [lancement ; incidents notables → leçon actée en une phrase].
- **[Date clé]** : [audit / refonte : constats chiffrés, décision prise, résultats].
- **[Date clé]** : [incident → correctif → validation du filet de sécurité].
- **[Date la plus récente]** : [dernier événement structurant, version publiée, prochaine bascule visée].

## 7. État courant & prochaines étapes (au [JJ/MM/AAAA])

*ℹ️ La photographie du présent : ce qui tourne, ce qui est en test, les 3 à 5 prochaines actions numérotées selon le backlog, et les chantiers de moyen terme.*

- **En production ([périmètre])** : [version, caractéristiques] — [sort prévu : conserver / décommissionner].
- **En test / beta ([périmètre])** : [version active, configuration].
- **Prochaines actions** (backlog du classeur) : [T-N : action → condition de passage] ; [T-M : action] ; [T-P : action (priorité)] ; [T-Q : échéance de continuité — ex. expiration de clé API le JJ/MM/AA].
- Chantiers moyen terme : [liste courte, chacun avec son déclencheur s'il existe].

## 8. Conventions de collaboration avec l'assistant IA (à respecter dans ce projet)

*ℹ️ Le contrat de travail entre vous et l'assistant : versionnage, procédures post-livraison, méthode, style attendu.*

- **Versionnage** : nomenclature [v X.Y.Z._suffixe → X.Y+1.0 à la bascule] ; toute livraison = [format exigé : fichier complet importable, validé], avec liste des changements.
- **Après chaque [import / déploiement]** : [checklist des re-configurations manuelles systématiques : credentials, réglages non exportés, données réinitialisées et leur compensation].
- **Méthode** : un changement de variable à la fois ; jamais de modification sur la production sans filet ; chaque affirmation factuelle importante vérifiée contre sources primaires ; toute défaillance documentée au Changelog du classeur de pilotage.
- **Style attendu** : [ex. chemins de clics exacts, chiffres vérifiés, franchise sur les erreurs — y compris celles de l'assistant, pas de complaisance].

---

## 9. Fichiers à ajouter à la base de connaissances du projet

*Règle d'or : une seule version de vérité par fichier — remplacer, ne jamais empiler les versions.*

| # | Fichier | Rôle dans le projet | Fréquence de rafraîchissement |
|---|---------|--------------------|-------------------------------|
| 1 | **[NOM]_Contexte_Projet.md** (ce document) | Mémoire centrale du projet | Après chaque décision structurante |
| 2 | **[Fichier source de vérité du processus — ex. workflow.json]** | Source de vérité opérationnelle : paramètres, garde-fous, câblage | À chaque nouvelle version |
| 3 | **[NOM]_Pilotage_complet.xlsx** | Backlog, Gantt, KPI, Changelog, Runbook, Continuité | Hebdomadaire (revue du [jour] [heure]) |
| 4 | **[Livrable de référence — ex. édition exemplaire du produit]** | Étalon : ton, format, niveau d'exactitude attendu | Remplacer si dépassé par une meilleure version |
| 5 | **[Archive de l'ancienne version]** | Archéologie et comparaisons | Figé — retirer [délai] après bascule |
| 6 | **[Document de conformité — quand rédigé (tâche N)]** | Cadre réglementaire / éditorial | À chaque révision |
| 7 | **[Documents stratégiques : pré-mortem, économie unitaire, personas, plan GTM]** | Fondations des décisions produit / prix | Figés |

Optionnel utile : un dossier « corpus de non-régression » — 2-3 livrables bloqués par les garde-fous (avec leur message d'erreur) comme exemples négatifs documentés.

## 10. Conversations à rattacher au projet

⚠️ **Comprendre d'abord ce que ça fait** : déplacer une conversation dans le projet (menu ⋮ de la conversation → *Change project* / *Ajouter au projet*) l'**organise** et la rend retrouvable par la recherche de conversations passées — mais son contenu n'est **pas** injecté automatiquement dans les nouveaux chats du projet. Seuls les fichiers de connaissances (§9) et les instructions le sont. C'est précisément pourquoi ce document existe : il distille les conversations en mémoire exploitable.

À rattacher, par ordre d'importance :

1. **[Conversation la plus dense — chantier fondateur]** : [ce qu'elle contient : architecture, décisions, incidents].
2. **[Construction du processus central]** : [versions, outils].
3. **[Stratégie produit]** : [pré-mortem, économie unitaire, go-to-market, personas].
4. **[Création du classeur de pilotage]** : [structure, conventions].
5. **[Lancement commercial & stack de vente]**.
6. **[Incident fondateur & sa résolution]** : [la leçon de discipline qui en découle].
7. **[Marketing / acquisition]**.
8. **[Conformité]**.
9. Optionnel — hors périmètre strict mais liées : [analyses connexes]. À rattacher seulement si le projet doit couvrir la stratégie au sens large ; sinon les laisser hors projet pour garder le contexte pur.

À **ne pas** rattacher : [projets voisins qui méritent leur propre espace].

## 11. Instructions personnalisées du projet (texte prêt à coller)

> Tu travailles sur [NOM DU PROJET] ([domaine]), [nature de l'activité] de [STRUCTURE], avec son fondateur ([profil : solo, techniquement autonome, non-développeur]). Le produit central est [PRODUIT], [mode de production résumé] décrit dans [NOM]_Contexte_Projet.md — lis-le avant toute réponse structurante, ainsi que [fichier source de vérité] et le classeur de pilotage pour l'état des tâches.
> Règles : (1) chemins de clics exacts pour toute manipulation ([outils concernés]) ; (2) tout chiffre ou fait important vérifié contre sources primaires, jamais de mémoire ; (3) un changement de variable à la fois, jamais de modification sur la production sans filet ; (4) tout livrable [type] = [format complet exigé], versionné selon la nomenclature en vigueur ; (5) conformité [cadre] : [interdit majeur] dans les livrables ; (6) discipline budgétaire : signaler tout choix qui augmente les coûts, proposer l'alternative frugale ; (7) rappeler la mise à jour du classeur de pilotage et du document de contexte après chaque changement structurant ; (8) franchise totale, y compris sur les erreurs passées de l'assistant.

## 12. Faire évoluer le niveau d'optimisation du projet

**Hygiène de base (dès la création)**
- Un chat = un sujet, nommé explicitement (« [Exemple 1] », « [Exemple 2] », « [Exemple 3] »). Les chats fleuve mélangent les contextes et diluent la recherche.
- Activer « Search and reference past chats » dans les réglages : les conversations rattachées deviennent interrogeables depuis les nouveaux chats.
- Après chaque changement structurant : rafraîchir les **3 fichiers vivants** (contexte, [source de vérité], classeur). C'est le geste qui maintient le projet « chaud ». Le classeur en est le journal ; ce document en est la synthèse.

**Niveau 2 — dans les semaines qui viennent**
- Extraire les [éléments clés du processus — ex. prompts système, paramètres critiques] dans un fichier lisible de la base de connaissances : itérer en discutant un document plutôt qu'en fouillant [le fichier technique].
- Créer un `Runbook_[Produit].md` : que faire à [heure critique] si alerte ([diagnostic, mode dégradé, repli, contacts]) — le pendant opérationnel du Runbook incidents du classeur.
- Coller chaque [jour de revue] dans un chat « Revue hebdo » : [coûts de la semaine, KPI, incidents] — l'assistant tient la revue avec l'historique du projet sous les yeux.

**Niveau 3 — optimisation continue**
- Constituer un **corpus de livrables** ([5-10 exemplaires datés]) dans la base de connaissances : base de non-régression (« compare le livrable du jour au corpus, signale les dérives »).
- Réévaluer trimestriellement : [outils et fournisseurs — arbitrer sur coût réel mesuré, jamais sur annonce], seuils des garde-fous ([les tolérances initiales sont des premières valeurs, à ajuster sur données]), et ce document lui-même (ce qui n'a plus cours part en « Chronologie », le présent reste court).

*Fin du document — version [1.0], [JJ/MM/AAAA].*
