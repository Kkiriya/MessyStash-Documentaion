# DA2M — Rapport de lancement du projet d’équipe

> Synthèse d’une séance autonome à compléter ensemble, puis à soumettre par le Scrum Master. Le groupe vérifie ses livrables à chaque étape. Utilisez les liens vers les fiches complétées pour les détails. Remplacez les indications entre crochets.

**Date de la séance :** 13 octobre 2026
**Mode :** travail autonome en équipe
**Équipe et application :** Neptune — MessyStash
**SM responsable de la remise :** Émile Valade

## 1. Liens obligatoires et documents

| Élément                                            | Lien exact                                                                                                       |
| -------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Organisation GitHub DA2M du cours                  | https://github.com/A26-DA2M                                                                                      |
| Repository de l’équipe dans cette organisation     | https://github.com/A26-DA2M/neptune/tree/main                                                                    |
| GitHub Project de l’équipe dans cette organisation | https://github.com/orgs/A26-DA2M/projects/4                                                                      |
| README                                             | https://github.com/A26-DA2M/neptune/blob/main/README.md                                                          |
| Fiche d’identité du produit complétée              | https://github.com/A26-DA2M/neptune/blob/docs/finishing-lancement-equipe/docs/Fiche_idee_%26_identite_produit.md |
| Persona principal et ses deux scénarios            | https://github.com/A26-DA2M/neptune/blob/docs/finishing-lancement-equipe/docs/Persona/P01-Alex.md                |
| Maquettes fournies utilisées et annotées           | [Lien]                                                                                                           |

**Propriétaire du repository :** A26-DA2M
**Propriétaire du Project :** A26-DA2M/neptune
**Accès de l’enseignante aux deux espaces :** Propriétaire de l'organisation

## 2. Équipe et responsabilités

L’équipe comprend obligatoirement 3 ou 4 membres. Désignez un PO et un SM distincts; tous contribuent au développement.

| Nom            | Identifiant GitHub | Responsabilités Scrum     | Première contribution technique précise    | Lien de la tâche                            | Aide ou relecture |
| -------------- | ------------------ | ------------------------- | ------------------------------------------ | ------------------------------------------- | ----------------- |
| Jean-Simon Cyr | Jaska28            | Product Owner + Developer | 1 Epic, 3 User Stories                     | https://github.com/orgs/A26-DA2M/projects/4 | Github Projet     |
| Émile Valade   | Kkiriya            | Scrum Master + Developer  | Redaction du rapport de lancement d'equipe | https://github.com/A26-DA2M/neptune         | Direct dans main  |
| Nerkesly       | Nerkesly           | Developer                 | Review Documentation                       | N/A                                         | Tout              |

**Pourquoi cette répartition convient-elle à l’équipe ?**
Cette répartition convient à l'équipe, car :

- **Jean-Simon** a plus ou moins assumé le rôle de _Product Owner_ auparavant. Il est sociable et habile dans les relations interpersonnelles.
- **Émile Valade** a choisi le rôle de _Scrum Master_ afin de développer ses compétences en gestion et de relever un nouveau défi.
- **Nerkesly** a pris le rôle de _Developer_, car c'était le seul poste restant.

## 3. Idée retenue et valeur

**Description en une phrase :**
**MessyStash** aide les particuliers à gérer et à organiser leur désordre grâce à une interface graphique intuitive qui permet de créer des `Boite` et d’y ajouter des `Objet`.

**Problème concret et valeur pour l’utilisateur :**

- **Situation actuelle et difficultés :**
  - Jean-Simon possède une boîte remplie de jeux vidéo, de consoles, de manettes, etc. Il souhaite pouvoir retrouver ses objets rapidement.
  - Il oublie assez souvent l’emplacement de certains objets lorsqu’il les cherche.

- **Amélioration apportée :**
  - Grâce à **MessyStash**, il lui suffit de rechercher un `Objet` dans l’application pour connaître son emplacement exact, notamment la pièce de la maison où il se trouve ainsi que la `Boite` dans laquelle il est rangé.

**Objectif de la première version :**
Un gestionnaire d’inventaire personnel fonctionnel qui intègre un système de codes QR permettant de retrouver et de consulter facilement les `Objet` enregistrés en scannant les codes à l’aide d’un téléphone intelligent.

**Fonctionnalités essentielles au MVP :**

- CRUD d'`Objet` et de `Boite`
- Gestion & Localisation de `Boite` et `Object`
- Generation et lecture de code QR

**Fonctionnalités reportées :**

- Intégration d’un agent LLM pour l’estimation de la valeur totale de l’inventaire.
- Optimisation du placement des `Objets` et de la création de `Boîtes` optimales.

**Persona principal :** [Identifiant et besoin principal]

Les détails sont dans les fiches d’identité et de persona liées à la section 1.

## 4. Trois pages et maquettes

| Page     | Besoin et contenu principal | Action de l’utilisateur | Navigation               | Maquette fournie utilisée |
| -------- | --------------------------- | ----------------------- | ------------------------ | ------------------------- |
| [Page 1] | [Contenu]                   | [Action]                | [Origine et destination] | [Lien et annotation]      |
| [Page 2] | [Contenu]                   | [Action]                | [Origine et destination] | [Lien et annotation]      |
| [Page 3] | [Contenu]                   | [Action]                | [Origine et destination] | [Lien et annotation]      |

**Parcours principal reliant les pages :**
[Suite d’actions, du déclencheur au résultat attendu.]

**Adaptations des maquettes au produit :**
[Contenus, actions et annotations ajoutés.]

## 5. Formulaire et backend

**Technologies prévues :** Flutter/Dart; Node.js/Express; MongoDB.
**Page du formulaire et donnée créée :** [Page — donnée]
**Champs et règles de validation :** [Résumé; détails dans la fiche d’identité ou la User Story]

| Opération                  | Requête envisagée | Données reçues ou retournées   | Résultat visible dans Flutter       |
| -------------------------- | ----------------- | ------------------------------ | ----------------------------------- |
| Consulter                  | GET [route]       | [Liste ou objet JSON]          | [Affichage]                         |
| Créer depuis le formulaire | POST [route]      | [Champs envoyés et objet créé] | [Confirmation et nouvelles données] |

**Données conservées dans MongoDB :** [Objet principal et champs]
**Persistance :** [Comment une donnée saisie est enregistrée puis retrouvée lors d’une nouvelle consultation]
**Erreur réseau ou serveur :** [Message, reprise possible et traitement de la saisie]

## 6. Début du backlog et critères d’acceptation

Utilisez les modèles pour les descriptions des issues et ajoutez toutes les issues au Project.

| Type       | Titre                      | Lien GitHub                                  | Parent | Priorité | Points US, si estimés |
| ---------- | -------------------------- | -------------------------------------------- | ------ | -------- | --------------------- |
| Epic       | E01: Manage Storage Boxes  | https://github.com/A26-DA2M/neptune/issues/1 | N/A    | HIGH     | -                     |
| User Story | US01: Create a Storage Box | https://github.com/A26-DA2M/neptune/issues/5 | E01    | MEDIUM   | 5                     |
| User Story | US02: View Storage Boxes   | https://github.com/A26-DA2M/neptune/issues/6 | E01    | MEDIUM   | 3                     |
| User Story | US03: Edit a Storage Box   | https://github.com/A26-DA2M/neptune/issues/7 | [Epic] | MEDIUM   | 3                     |
| User Story | US04: Delete a Storage Box | https://github.com/A26-DA2M/neptune/issues/8 | [Epic] | MEDIUM   | 2                     |

Les tâches techniques et leurs responsables figurent à la section 2. Chaque tâche renseigne ses labels, sa priorité, ses critères de fin et son poids estimé, ou la question qui empêche encore l’estimation.

**Ordre des User Stories et justification du PO :** [Ordre et valeur]
**Questions d’estimation des Developers :** [Hypothèses et points à clarifier, ou Aucune]

Dans les User Stories, préciser les critères d’acceptation du parcours : consultation, navigation, enregistrement valide, saisie invalide, erreur de communication et données retrouvées après réouverture.

**Deux critères représentatifs de notre application :**

- [Situation ou action → résultat observable attendu — lien de la User Story]
- [Cas limite ou erreur → résultat observable attendu — lien de la User Story]

## 7. Accords de fonctionnement et première DoD

Définissez 3 à 5 règles concrètes.

| Sujet                          | Accord                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Communication et disponibilité | **Canal :** Groupe Discord, <br> **Moment d’échange :** Mercredi 18:00, <br> **délai de réponse convenu :** _1h_ à _3h_ la semaine, _1 jours ouvrable_ la fin de semaine                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Mise à jour du board           | **Backlog :** Tâches à faire. On y ajoute toutes les nouvelles tâches créées. <br> **Ready :** Tâches prêtes à être exécutées. On y ajoute les tâches qui n’ont aucune dépendance et qui sont prêtes à être implémentées. <br> **In Progress :** Tâches en cours. On y déplace une tâche lorsqu’un membre de l’équipe la prend en charge. <br> **In Review :** Tâches en attente de révision. On y ajoute les tâches qui viennent d’être terminées. Elles y restent jusqu’à ce qu’un autre développeur les révise et les approuve. <br> **Done :** Tâches terminées. On y déplace les tâches lorsqu’elles sont entièrement complétées, révisées et approuvées. |
| Relecture et intégration       | Aucune **pull request** ne peut être acceptée sans avoir fait l’objet d’une révision par un pair (_peer review_). <br> Chaque **pull request** doit contenir au moins un commentaire pertinent. <br> Chaque commit doit respecter la convention établie par l’équipe (`path/to/file`).                                                                                                                                                                                                                                                                                                                                                                         |
| Blocage, désaccord ou absence  | Signaler tout blocage, désaccord ou toute absence au **Scrum Master**. <br> En cas de non-réponse du **Scrum Master** ou d’impossibilité de parvenir à une entente, faire remonter la situation au **Product Owner**.                                                                                                                                                                                                                                                                                                                                                                                                                                          |

**Prochain point d’équipe :** Mercredi 21 octobre à 18 h.

**Definition of Done commune :**

- **Code fonctionnalité :** La fonctionnalité est entièrement implémentée, fonctionne comme prévu et respecte les critères d’acceptation définis dans la User Story.
- **Tests et validation :** La fonctionnalité a été testée et ne présente aucun bogue majeur connu. Les tests pertinents doivent être réussis.
- **Revue de code :** Le code a été révisé et approuvé par au moins un autre membre de l’équipe avant la fusion de la Pull Request dans la branche principale.
- **Documentation et intégration :** Le code respecte les conventions établies par l’équipe, la documentation pertinente est à jour et la fonctionnalité est intégrée sans compromettre les fonctionnalités existantes.

**Lien vers cette DoD à utiliser dans les issues :** [Lien de cette section sur GitHub]

## 8. Prochaines actions et questions

| Prochaine action                                        | Membre qui la prend | Résultat attendu                       | Moment cible convenu |
| ------------------------------------------------------- | ------------------- | -------------------------------------- | -------------------- |
| Paufiner le kanban                                      | Jean-Simon          | Tableau Kanban propre                  | 1 semaine            |
| Migrer la documentation vers github wiki + architecture | Émile Valade        | github wiki + diagramme d'architecture | 1 semaine            |
| Lire la documentation                                   | Nerkesly            | N/A                                    | 1 semaine            |

**Organisation du travail autonome :** [Comment le groupe a réparti le travail, suivi les étapes et vérifié les résultats; rôle du SM dans cette facilitation.]

**Décisions principales et raisons :** [Résumé des choix faits ensemble.]

**Questions à l’enseignante après la remise :** [Questions ou Aucune]
**Hypothèses à confirmer :** [Hypothèse, action de vérification et membre qui la prend, ou Aucune]
**Blocages :** [Cause, essais effectués, signalement envoyé si nécessaire et prochaine action, ou Aucun]

## 9. Validation collective et remise

- [x] Nous sommes 3 ou 4 membres, avec un PO et un SM distincts.
- [x] Chaque membre a une contribution technique et une issue associée.
- [x] Nous avons vérifié les résultats à chaque étape et consigné nos questions.
- [x] Tous les membres ont relu et approuvé le rapport.
- [ ] Les modèles et les maquettes fournis sont utilisés.
- [x] Notre idée couvre trois pages, une navigation, un formulaire et un backend avec persistance.
- [x] Les deux espaces GitHub existent dans l’organisation DA2M, sont reliés et accessibles à l’enseignante.
- [x] Le backlog contient au moins 1 Epic, 3 User Stories et 1 tâche par membre, avec les informations demandées.
- [x] Le rapport est dans le dépôt et le README permet de retrouver les documents et le Project.
- [x] Le SM a soumis le rapport et les deux liens dans l’espace de remise indiqué.

**Membres ayant validé :** Jean-Simon Cyr
**Remise effectuée par :** Émile Valade
**Date et heure :** 20/10/26 16:15

## 10. Retour de l’enseignante — après la remise

**Proposition :** [Acceptée / Ajustements demandés / À discuter]
**Commentaire et suite convenue :** [Retour et prochaine action]

Ce travail est non noté, mais obligatoire et essentiel à la progression du projet.
