## Introduction

Ce document décrit l'approche de développement logiciel Start.dev et les termes de collaboration avec des freelances (ingénieurs logiciels/développeurs/propriétaires de produits) appelés "Partenaires" dans ce document. Il s'appuie sur la méthodologie Agile Scrum (les détails sont disponibles ici) et le développement logiciel Agile Trello pour construire 7 éléments de gouvernance tels que :

- Le processus de collaboration au sein Start.dev ;
- Les outils de collaboration ;
- Le workflow ;
- Les cartes Trello :
  - Les étiquettes ;
  - La hiérarchie ;
  - La documentation ;
  - L'archivage.
- La définition d'un travail de développement "TERMINÉ", c'est-à-dire "FACTURABLE" ;
- Le processus de gestion du code ;
- Le glossaire.

Nous définissons ensuite chaque élément dans des sections dédiées.

### Processus de Collaboration au sein Start.dev

Start.dev encourage une mentalité axée sur les résultats, établit des partenariats centrés sur le produit et lutte fortement contre les attitudes axées sur les tâches. Cela implique une corrélation entre la livraison du produit et la facturation. Par conséquent, nous ne nous attendons pas à payer les partenaires pour le travail (les moyens) mais pour ses résultats (les résultats). De plus, nous encourageons nos PARTENAIRES À NOUS AIDER À CONSTRUIRE DES PRODUITS ET NON À CODER À L'AVEUGLE!

Un "contrat de livraison" entre un partenaire et Start.dev contient les 4 termes suivants :

- Les objectifs et les résultats attendus d'un travail : incréments de produits (par exemple, fonctionnalité, histoires d'utilisateur, modules, etc.) ou résultats attendus pour les activités de gestion (par exemple, tâches du propriétaire de produit pendant un Sprint) ;
- Les critères d'acceptation pour considérer que les objectifs sont atteints ;
- Le coût de la livraison en nombre de Jours-Homme (8 heures de travail) : 3 Jours-Homme/résultats pour les résultats de développement ;
- La date limite.

Respecter ces termes contractuels déclenche le paiement. En résumé, nous ne payons pas pour les heures passées à effectuer des tâches mais pour les résultats attendus de celles-ci. Concrètement, pour toute livraison de développement, le travail doit être :

- Qualifié par les Product Owners et les Développeurs :
  - Objectifs définis par les propriétaires de produits ;
  - Critères d'acceptation décrits et convenus entre le développeur et le propriétaire de produit.
- Tarifié :
  - Le nombre de jours-homme proposé par le développeur ;
  - Le nombre de jours-homme transféré par le propriétaire de produit au Fondateur Start.dev (Phidias) ;
  - La tarification acceptée par le Fondateur Start.dev (Glaine & Phidias).
- Planifié :
  - Lors d'une planification de Sprint ;
  - Les tickets sont créés dans le logiciel Trello avant de commencer le développement comme expliqué dans la section Workflow.
- Finalisé comme expliqué dans la section Définition d'un travail de développement "Terminé", c'est-à-dire facturable ;
- Présenté lors d'une démo lors d'une revue de Sprint.

### Outils de Collaboration

Le tableau ci-dessous décrit les outils utilisés par Start.dev.

| Outils      | Objectifs                         | Qui peut accorder l'accès aux nouveaux ? |
|-------------|-----------------------------------|-----------------------------------------|
| Trello      | Outil de gestion agile            | Moasko dev                        |
| Google Drive| Stockage de documents             | moasko dev                       |
| Slack       | Canaux de communication           | Tout le monde                           |
| Github      | Gestion du code / Pipeline CI-CD  | Moasko dev                                 |

### Workflow

Le flux de travail de développement comprend 8 voies comme illustré dans la capture d'écran ci-dessous :

- Product Backlog ;
- Sprint Backlog ;
- Ongoing ;
- Blocking ;
- Paused ;
- To Review ;
- Done ;
- Cancelled.

#### Product Backlog

La voie Product Backlog contient toutes les cartes que le Product Owner ou tout membre de l'équipe crée pour garder une trace d'une idée liée à la construction du logiciel. Par exemple, lors d'une réunion quotidienne, une discussion a souligné la nécessité d'améliorer une fonctionnalité logicielle. Ensuite, le propriétaire de produit ou tout membre l'enregistre sur une carte stockée dans cette voie. D'autres exemples de cartes stockées dans cette voie sont les Epics ou les Initiatives (décrites dans la section Trello Card, précisément dans la sous-section Hiérarchie) qui regroupent les histoires et les tâches (par exemple, modules, versions ou fonctionnalités du projet).

#### Sprint Backlog

La voie Sprint Backlog contient le travail planifié au début d'un Sprint. Il contiendrait des tâches, des documents ou des histoires à réaliser au début du Sprint. Dans la section Trello Card (Sous-section Hiérarchie), nous verrons qu'une carte de tâche doit être liée à une histoire correspondant aux fonctionnalités du produit. En général, la réunion de planification du Sprint vise à définir les priorités et à sélectionner les histoires ou/et les tâches à réaliser. En conséquence, le développeur doit créer en amont dans Trello toutes ses tâches pour le Sprint.

#### Ongoing

La voie Ongoing comprend le travail en cours de tous les membres de l'équipe pendant un sprint. En d'autres termes, lorsqu'un développeur ou tout membre de l'équipe est occupé sur une tâche, une carte liée à son nom devrait être disponible là-bas. Idéalement, une carte par membre de l'équipe devrait être visible à un moment précis si l'on suppose que quelqu'un ne peut pas travailler simultanément sur plus d'une tâche. Nous recommandons fortement de travailler sur une tâche à la fois et de la compléter avant de commencer une nouvelle.

#### Blocked

La voie Blocked inclut la carte qui ne peut pas être terminée en raison d'extériorités ou de dépendances rencontrées par le partenaire. Par exemple, pour réaliser la tâche, les ingénieurs auraient besoin de clarifications du propriétaire de produit ou ils ont besoin qu'un fondateur Start.dev achète un plugin.

#### Paused

La voie Paused contient les tâches non terminées. Pendant le sprint, le partenaire pourrait ne pas être disponible ou il pourrait travailler sur une tâche avec une priorité plus élevée. Cependant, cela doit être exceptionnel, une fois de plus, nous recommandons fortement à notre partenaire de travailler sur une tâche à la fois et de s'assurer de la terminer avant d'en commencer une nouvelle.

#### To Review

La voie To Review contient le travail de développement réalisé mais non considéré comme "Terminé". D'une part, cela signifie que la partie codage a été réalisée et doit maintenant être examinée par des pairs. D'autre part, le propriétaire de produit doit évaluer l'incrément de produit par rapport aux critères d'acceptation de la tâche ou/et des histoires.

#### Done

Les cartes peuvent être dans la voie Done lorsqu'elles répondent aux conditions de la section Définition d'un travail de développement "Terminé", c'est-à-dire facturable.

#### Cancelled

La section Cancelled contient les cartes créées par erreur ou hors du périmètre.

### Cartes Trello

#### Étiquettes

La gouvernance du développement fait un usage extensif des étiquettes. En plus du texte affiché dans l'étiquette, une couleur de code permet de spécifier son objectif.

Le tableau ci-dessous décrit le code couleur de l'étiquette de carte. Considérant que la coloration des cartes n'est pas une science exacte, tout partenaire est autorisé à ajuster la liste des valeurs de toute couleur pour faciliter son travail. Cependant, il doit informer tous les membres de l'équipe du changement et de ses motivations.

### Étiquettes de cartes Trello

| Couleur | Objectif | Valeur |
|-------------|--------------------------------------------------|----------------------------------|
| ![#00ff00](https://placehold.co/10x25/00ff00/00ff00.png) Vert | Type de carte | Document, Epic, Initiative, Story, Sub-Task, Task |
| ![#ffa500](https://placehold.co/10x25/ffa500/ffa500.png) Orange | Temps alloué pour réaliser une tâche | 2 Heures, 4 Heures |
| ![#ff0000](https://placehold.co/10x25/ff0000/ff0000.png) Rouge | Importance et urgence de la tâche pour le Sprint | IMPORTANT, URGENT |
| ![#800080](https://placehold.co/10x25/800080/800080.png) Violet | Détails des tâches | Analysis, Code Review, Deployment, Design UX/UI, Development, Document, Product Management, Release, Testing |
| ![#00008b](https://placehold.co/10x25/00008b/00008b.png) Bleu Foncé | Spécifications du travail de développement | Bug, Improvement, New Feature, Refactoring |
| ![#add8e6](https://placehold.co/10x25/add8e6/add8e6.png) Bleu Clair | Partie technique des applications | Frontend, Backend, CI/CD Platform, Data Platform |
| ![#ff69b4](https://placehold.co/10x25/ff69b4/ff69b4.png) Rose | Numéro de la première semaine du Sprint | Sprint 40, Sprint 42, Sprint 44 |



#### Hiérarchie

Les termes présents dans les "étiquettes vertes" permettent la hiérarchie entre les cartes comme expliqué et illustré dans l'image provenant du site web.

Les types de cartes Trello (illustrés dans la capture d'écran ci-dessous) sont présentés par ordre décroissant :

- Initiative : correspond au plus haut niveau d'un projet de développement. Par exemple, la création d'une version du logiciel telle que le Minimum Viable Product (MVP) ou une nouvelle version pour soutenir le cas d'utilisation d'un nouveau projet.
- EPIC : une énorme histoire ou des blocs de construction d'une Initiative ;
- Story : traduction des exigences ou attentes des produits ou des clients ; description des fonctionnalités ; détails des fonctionnalités.
- Task : unités de travail facturable nécessaires pour réaliser une histoire. Le temps alloué pour réaliser une tâche est compris entre 2 et

 4 heures ;
- Sub-Task : unités de travail facturable nécessaires pour réaliser une histoire. Le temps alloué pour réaliser une sous-tâche est compris entre 2 et 4 heures ;
- Meeting : carte utilisée pour enregistrer les réunions.

Les "meilleures pratiques" de création de cartes (résumées dans le tableau ci-dessous) impliquent le schéma suivant :

- Les Initiatives doivent contenir uniquement des EPICs et être gérées par les Fondateurs/Product Owners Start.dev ;
- Les EPICs doivent contenir uniquement des Stories et être créées par le Product Owner (toutefois, dans certains cas, des Tasks peuvent également être incluses) ;
- Les Stories doivent contenir uniquement des Tasks et être créées par le Product Owner ou son représentant (Analyste) ;
- Les Tasks doivent contenir uniquement des Sub-Tasks et être créées par le partenaire réalisant les tâches.

| Carte       | Propriétaire                               | Contient                     | Voie               |
|-------------|--------------------------------------------|------------------------------|--------------------|
| Initiative  | Fondateurs/Product Owners Start.dev          | EPICs                        | Product Backlog    |
| EPIC        | Product Owner                              | Stories                      | Product Backlog    |
| Story       | Product Owner                              | Tasks                        | Partout            |
| Task        | Partenaire (Product Owner ou Développeur)  | Sub-Tasks                    | Partout            |
| Sub-Task    | Partenaire (Product Owner ou Développeur)  | Non applicable               | Partout            |

Le propriétaire de la tâche est responsable de A à Z de sa documentation appropriée comme expliqué dans la section suivante.

#### Documentation

Nous utilisons de bons exemples de types de cartes pour proposer les spécifications de leur documentation :

- Initiative ;
- EPIC ;
- Story ;
- Task.

##### Initiative

[Exemple d'initiative](https://trello.com/c/bA7YdhOR/13-leisure-experience-mvp)

##### EPIC

[Exemple d'EPIC](https://trello.com/c/1JIIfKMk/19-discover-leisure-experience)

##### Story

[Exemple de Story](https://trello.com/c/7yVLCckq/124-top-global-search-look-for-activities-or-events)

La description de l'histoire utilisateur doit suivre le modèle ci-dessous :

En tant que <type d'utilisateur>, je veux <un objectif> afin de <une raison>.

Utilisez la méthode INVEST : [Méthode INVEST](https://agileforall.com/new-to-agile-invest-in-good-user-stories/)

Nous utilisons l'approche BDD pour détailler les spécifications de l'histoire et les critères d'acceptation : [Approche BDD](https://docs.google.com/presentation/d/19vmwfKYiqzc8aiiFA_J63QqpllQYR8lnj5iiwgNH6fg/edit#slide=id.p)

##### Task

[Exemple de Task](https://trello.com/c/IwCTDDiv/260-fix-bug-research-by-location-research-list-filter)

#### Archivage

Les cartes dans les voies Done et Cancelled seront archivées afin de nettoyer le tableau Trello.

### Définition d'un travail de développement "TERMINÉ", c'est-à-dire "FACTURABLE"

Le partenaire peut facturer Start.dev en fonction du tarif décrit ci-dessous :

- Tâches
  - Minimum : 2 heures
  - Maximum : 4 heures
  - 1 jour-homme = 8 heures passées sur des tâches assignées par Start.dev
  - Min 2 tâches/jour
  - Max : 4 tâches/jour
  - Tarif : 20000 FCFA/jour

Start.dev paiera les factures pour le travail considéré comme "TERMINÉ". Un travail est "TERMINÉ", c'est-à-dire facturable et payable, lorsqu'il répond aux critères ci-dessous :

- Testé : tests unitaires, de régression et d'intégration ;
- Revu par des pairs à l'aide de "Pull Request" (cycle de "révision, correction et soumission") ;
- Intégré à la branche demandée (par exemple, develop, feature ou hot-fix) ;
- Documenté dans la carte Trello Task et la Pull Request,
  - Le but du développement réalisé ;
  - La manière dont le but est atteint à travers le code ;
  - Les tests unitaires, les tests de régression et les tests d'intégration ;
  - Le plan de test et les résultats basés sur les critères d'acceptation convenus avec le Product Owner.
- Accepté par le Product Owner que l'incrément de produit/fonctionnalité répond aux critères d'acceptation.

Voir la carte [Exemple de carte Trello](https://trello.com/c/IwCTDDiv/260-fix-bug-research-by-location-research-list-filter)

Le partenaire est responsable de rendre le travail "TERMINÉ" et Start.dev DOIT LE PAYER en conséquence.

#### Tests unitaires contre le scénario Gherkin

Le développeur DOIT effectuer des tests unitaires contre les scénarios écrits avec la syntaxe Gherkin (voir l'exemple ci-dessous). Le scénario DOIT spécifier les fonctionnalités impactées par le scénario.

**Exemple de scénario Gherkin**

```gherkin
Feature: Account Holder withdraws cash

Scenario: Account has sufficient funds
  Given The account balance is $100
    And the card is valid
    And the machine contains enough money
  When the Account Holder requests $20
  Then the ATM should dispense $20
    And the account balance should be $80
    And the card should be returned
```

[Syntaxe Gherkin](https://docs.behat.org/en/v2.5/guides/1.gherkin.html)

### Processus de Gestion du Code

[Gitflow Workflow](https://www.atlassian.com/fr/git/tutorials/comparing-workflows/gitflow-workflow)

### Glossaire

[Glossaire](https://docs.google.com/spreadsheets/d/1tAFeHodyvqHR12WNC2Yru4Y6AG7Y0BY5vgjb1gChQnI/edit#gid=0)
