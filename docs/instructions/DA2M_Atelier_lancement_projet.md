# DA2M — Atelier de lancement du projet d’équipe

**Durée :** 3 heures
**Mode :** travail autonome en équipe; chaque groupe suit les étapes et gère son rythme.
**Séance :** 13 octobre 2026
**Travail :** en équipe de 3 à 4 membres, obligatoire et non noté
**Remise :** à la fin de la séance, par le Scrum Master, dans l’espace Teams indiqué par l’enseignante

**Organisation GitHub DA2M :** lien fourni dans les ressources de la séance.
**Maquettes et modèles à utiliser :** ressources remises par l’enseignante.

## 1. Objectif de la séance

Vous devez vous entendre sur le produit que vous développerez dans DA2M et sur votre façon de travailler ensemble. À la fin de la séance, chaque membre doit pouvoir expliquer le besoin auquel répond l’application, les responsabilités de chacun et sa prochaine contribution technique.

Vous produirez une proposition de projet, un début de backlog et un environnement GitHub commun. Le développement de l’application se poursuivra pendant le cours. Aujourd’hui, vous devez décrire et organiser les fonctionnalités attendues; l’application complète sera réalisée ensuite.

Cette activité prépare le travail en Sprints. Consignez vos choix dans les documents; l’enseignante donnera un retour sur votre proposition après la remise.

### Comment conduire cette séance en autonomie

1. Chaque membre lit les consignes et ouvre les ressources : modèles, maquettes, lien de l’organisation GitHub et espace de remise.
2. En formant l’équipe, choisissez une personne pour suivre le temps jusqu’à la désignation du Scrum Master.
3. Une fois désigné, le SM facilite les échanges, veille à la participation de chacun et aide le groupe à suivre le calendrier de la section 8.
4. Répartissez la rédaction et la configuration en parallèle. À la fin de chaque étape, vérifiez ensemble le résultat attendu avant de poursuivre.
5. Consignez vos décisions et les questions à clarifier dans le rapport. Pour une question qui permet de poursuivre, notez votre hypothèse et la vérification à prévoir.
6. Réservez les 25 dernières minutes à la relecture, aux liens et à la remise par le SM.

Le SM facilite le travail collectif. Le PO porte les décisions produit et les Developers organisent le travail technique; chacun participe aux échanges et à la réalisation.

## 2. Former l’équipe et répartir les responsabilités Scrum

**Chaque équipe comprend obligatoirement 3 ou 4 membres. Cette contrainte est non négociable.**

Votre équipe désigne **un Product Owner et un Scrum Master, deux personnes distinctes**. Tous les membres contribuent au développement, y compris le PO et le SM. La remise du rapport par le SM est une consigne de cette activité.

| Membre                         | Responsabilités Scrum dans l’équipe | Responsabilités concrètes                                                                                                                                                  |
| ------------------------------ | ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Membre 1                       | Product Owner + Developer           | Porter la vision, clarifier les besoins et les critères d’acceptation, ordonner le backlog; prendre aussi des tâches techniques.                                           |
| Membre 2                       | Scrum Master + Developer            | Faciliter les échanges, aider à traiter les obstacles et à utiliser le board; prendre aussi des tâches techniques; rassembler et soumettre le rapport validé par l’équipe. |
| Membre 3                       | Developer                           | Participer aux estimations, au découpage, à la réalisation, aux vérifications et à l’intégration.                                                                          |
| Membre 4, pour une équipe de 4 | Developer                           | Participer aux mêmes responsabilités de développement, selon la répartition convenue.                                                                                      |

Les Developers organisent ensemble le travail technique. Le SM facilite cette organisation; chaque membre tient ses propres issues à jour. Les responsabilités techniques peuvent être partagées et évoluer.

Complétez la répartition nominative dans le rapport :

- nom et identifiant GitHub de chaque membre;
- responsabilités Scrum;
- première contribution technique précise;
- lien vers la tâche prise en charge;
- personne pouvant aider ou relire ce travail.

Définissez également **3 à 5 règles d’équipe** : communication, disponibilité, suivi des issues, relecture et traitement d’un désaccord ou d’un blocage.

## 3. Choisir une application adaptée à DA2M

Votre application doit répondre à un besoin simple, pour un public clairement identifié. Choisissez une première version réalisable, appelée MVP.

Chacun présente une proposition en quelques phrases. Comparez les idées selon le besoin, l’utilité des trois pages, le formulaire, le backend et la faisabilité. Retenez ensemble une proposition, puis le PO en synthétise la vision dans la fiche d’identité.

### Exigences du produit à développer

| Élément          | Minimum attendu dans l’application                                                                                                  |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Frontend mobile  | Application Flutter/Dart.                                                                                                           |
| Pages            | Au moins **3 pages distinctes et utiles**, avec un contenu et une action clairement identifiés.                                     |
| Navigation       | Passage fonctionnel entre ces pages et retour cohérent dans le parcours.                                                            |
| Formulaire       | Au moins un formulaire utile au produit, avec validation des saisies et envoi au backend. Il peut constituer l’une des trois pages. |
| Backend          | API Node.js/Express réellement utilisée par Flutter.                                                                                |
| Données          | Persistance avec MongoDB et données retrouvées lors d’une nouvelle consultation.                                                    |
| Parcours complet | Au moins une lecture de données et une création à partir du formulaire, avec retour visible dans l’application.                     |

Dans votre proposition, nommez les trois pages, les champs du formulaire, les données principales et les opérations attendues du backend. Décrivez aussi ce que l’utilisateur verra si une saisie est invalide ou si la communication avec le serveur échoue.

### Exemples de projets acceptables

Ces idées respectent le minimum demandé si vous réalisez le parcours et la persistance décrits.

| Idée                       | Trois pages possibles                                            | Formulaire                       | Fonction du backend                                                      |
| -------------------------- | ---------------------------------------------------------------- | -------------------------------- | ------------------------------------------------------------------------ |
| Carnet de recettes         | Liste des recettes; détail d’une recette; ajout d’une recette    | Titre, ingrédients et étapes     | Enregistrer les recettes et les retourner à l’application.               |
| Bibliothèque personnelle   | Liste des livres; fiche d’un livre; ajout d’un livre             | Titre, auteur et état de lecture | Enregistrer et consulter les livres.                                     |
| Carnet d’activités locales | Liste des activités; détail d’une activité; ajout d’une activité | Nom, lieu et description         | Enregistrer et consulter les activités.                                  |
| Planificateur de révisions | Liste des séances; détail d’une séance; création d’une séance    | Matière, sujet et date           | Enregistrer et consulter les séances prévues.                            |
| Gestionnaire de tâches     | Liste des tâches; détail d’une tâche; création d’une tâche       | Titre et description             | Enregistrer et consulter les tâches; changement d’état possible ensuite. |

Vous pouvez proposer une autre idée répondant aux mêmes exigences. Le nom de l’application et son apparence doivent correspondre à votre public.

Un écran d’accueil décoratif, une page « À propos » ou un formulaire sans enregistrement ne suffisent pas à démontrer le parcours demandé. Les trois pages doivent contribuer au besoin du produit.

## 4. Réutiliser les maquettes et les modèles fournis

Utilisez les ressources remises par l’enseignante comme point de départ.

| Modèle Markdown                     | Utilisation pendant cette séance                                                   |
| ----------------------------------- | ---------------------------------------------------------------------------------- |
| `01_Idee_et_identite_du_produit.md` | Décrire l’idée, le problème, le public, la valeur, le MVP et les choix techniques. |
| `02_Persona.md`                     | Préparer un persona principal et ses deux scénarios d’utilisation.                 |
| `03_Epic.md`                        | Décrire au moins une Epic cohérente avec le besoin principal.                      |
| `04_User_Story.md`                  | Décrire les premières User Stories et leurs critères d’acceptation.                |
| `05_Tache_technique.md`             | Décrire les premières contributions techniques et leurs critères de fin.           |

Pour les **maquettes d’écrans fournies**, repérez et annotez les trois pages retenues : contenu, actions, champs du formulaire, liens de navigation et retours attendus. Adaptez le contenu à votre application tout en conservant les indications demandées. Ajoutez les fichiers ou leurs liens dans le dépôt et dans la fiche d’identité du produit.

Les fiches constituent une première version. Renseignez les éléments connus; pour un point encore incertain, écrivez une question précise et la prochaine action permettant de la résoudre.

## 5. Créer les deux espaces GitHub dans l’organisation DA2M

Votre équipe doit disposer de **deux éléments existants appartenant à l’organisation du cours** :

1. un **repository** pour le code et les documents;
2. un **GitHub Project** pour le suivi du backlog et du travail.

### Repository

- Créez ou utilisez le dépôt de votre équipe dans l’organisation DA2M.
- Lors de la création, vérifiez que le champ **Owner** désigne l’organisation du cours.
- Utilisez un nom clair, par exemple `da2m-nom-equipe`.
- Respectez la visibilité indiquée par l’enseignante.
- Vérifiez que les membres peuvent contribuer et que l’enseignante peut consulter le dépôt.
- Ajoutez un README avec le nom, une présentation courte du produit, les membres et leurs responsabilités, le lien du Project et les liens des documents.

Placez la fiche d’identité, le persona, le rapport et les maquettes dans un dossier `docs/`. Les Epics, User Stories et tâches sont suivies dans les issues du dépôt, avec les descriptions tirées des modèles.

### GitHub Project

- Depuis l’organisation DA2M, ouvrez **Projects**, puis créez ou utilisez le Project de votre équipe.
- Choisissez une vue **Board** et les statuts : **Backlog, To Do, In Progress, Done**.
- Reliez le Project au dépôt. Depuis le dépôt, cette association peut se faire dans **Projects → Link a project**.
- Ajoutez les issues du dépôt au Project.
- Vérifiez les droits de contribution des membres et l’accès de l’enseignante aux deux espaces.

Le Project et le repository ont chacun leur propre lien. Les deux seront remis.

Si un droit manque, le SM consigne le blocage et envoie un signalement précis dans le canal de cours indiqué : lien de l’espace concerné, action tentée et message d’erreur. Le propriétaire attendu reste l’organisation DA2M. Pendant la résolution, l’équipe poursuit les fiches, les maquettes et les descriptions d’issues.

Pour une difficulté, consultez d’abord les consignes, les modèles et les références en fin de document. Notez les essais effectués et la prochaine action dans le rapport. Les questions sur la proposition de produit seront examinées après la remise.

## 6. Amorcer le backlog et définir qui prend quel travail

Pour cette première séance, créez au minimum :

- **1 Epic** décrivant le grand besoin;
- **3 User Stories** couvrant les premiers résultats utiles, dont la consultation de données et la création via le formulaire;
- **1 tâche technique par membre**, donc 3 ou 4 tâches, reliées aux User Stories concernées.

Ce minimum sert à commencer le backlog. Vous l’enrichirez pendant le cours.

Chaque User Story contient la formulation « En tant que…, je veux…, afin de… », la valeur pour l’utilisateur et des critères d’acceptation vérifiables. Préparez le cas réussi, une limite ou saisie invalide pertinente et un comportement en erreur.

Chaque tâche décrit un livrable technique précis, ses critères de fin et le membre qui prend ce travail. Veillez à couvrir le frontend, le backend et leur intégration dans la répartition de l’équipe.

| Type d’issue | Label de type | Informations à renseigner                                                                                         |
| ------------ | ------------- | ----------------------------------------------------------------------------------------------------------------- |
| Epic         | `type:epic`   | Besoin, valeur, périmètre, critères d’acceptation globaux et priorité.                                            |
| User Story   | `type:story`  | Formulation, critères d’acceptation, Epic parente, priorité et première estimation si possible.                   |
| Tâche        | `type:task`   | Travail technique, critères de fin, User Story parente, priorité, responsable et première estimation si possible. |

Ajoutez aux tâches les labels techniques utiles : `frontend`, `backend`, `database`, `test` ou `configuration`.

Le PO ordonne les besoins : **P1 haute, P2 normale, P3 basse**. Les Developers proposent les estimations relatives, selon l’échelle des modèles : **1, 2, 3, 5, 8**. Si une estimation manque encore, indiquez « À estimer » dans la description avec la question à clarifier.

Si vous utilisez les champs numériques de Projects, les User Stories portent **Points US** et les tâches portent **Poids tâche**. Laissez l’autre champ vide; laissez les deux vides sur les Epics. Une estimation encore inconnue laisse le champ numérique vide.

Reliez les éléments par les relations de parent et sous-issues, ou au minimum par des liens explicites. Ajoutez toutes les issues au Project. Les fonctionnalités prévues restent dans **Backlog** jusqu’à leur sélection pour le travail. Chaque membre met ensuite ses cartes à jour selon l’avancement réel.

Les Epics, les User Stories, les labels et les points sont les conventions de suivi retenues pour le cours.

## 7. Préparer vos critères de qualité

Décrivez une première **Definition of Done commune** dans le rapport : quelques exigences de qualité que l’équipe appliquera aux fonctionnalités développées.

Vous pouvez partir de ces exigences et les préciser :

- les critères d’acceptation de la User Story sont vérifiés;
- le parcours Flutter–API–MongoDB fonctionne lorsque la fonctionnalité en dépend;
- les saisies invalides et les erreurs prévues sont traitées;
- le changement est relu par un autre membre et intégré dans le dépôt commun;
- les vérifications réalisées et les instructions utiles sont consignées.

Les critères d’acceptation décrivent le résultat propre à une fonctionnalité; la DoD décrit la qualité commune attendue.

## 8. Déroulement des trois heures

Les temps sont comptés depuis le début de votre période de travail. Le SM aide l’équipe à respecter ces repères. Chaque groupe effectue lui-même les vérifications de passage.

| Temps         | Durée  | Travail de l’équipe                                                                              | Résultat à vérifier ensemble                                                                        |
| ------------- | ------ | ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| 0 à 10 min    | 10 min | Lire les consignes et ouvrir les ressources.                                                     | Chaque membre connaît le résultat attendu et retrouve les modèles, maquettes et liens.              |
| 10 à 30 min   | 20 min | Former l’équipe, désigner PO et SM, répartir les premières responsabilités et écrire les règles. | 3 ou 4 membres; PO et SM distincts; contribution technique prévue pour chacun.                      |
| 30 à 65 min   | 35 min | Comparer les idées; compléter l’identité du produit et le persona principal.                     | Chacun peut expliquer le public, le problème, la valeur et le MVP retenus.                          |
| 65 à 85 min   | 20 min | Annoter les trois pages, la navigation, le formulaire et les opérations du backend.              | Le parcours et la persistance sont décrits et reliés aux maquettes.                                 |
| 85 à 95 min   | 10 min | Pause.                                                                                           | L’équipe reprend à l’heure convenue.                                                                |
| 95 à 125 min  | 30 min | Mettre en place le dépôt et le Project dans l’organisation; déposer les documents.               | Les deux espaces appartiennent à DA2M; les membres peuvent contribuer et le README donne les liens. |
| 125 à 155 min | 30 min | Créer le premier backlog avec les modèles et attribuer les tâches.                               | 1 Epic, 3 User Stories et 1 tâche par membre; critères et liens présents.                           |
| 155 à 180 min | 25 min | Compléter et relire le rapport; contrôler la liste de vérification; remettre par le SM.          | Tous ont relu; les deux liens existent et la remise du SM est effectuée.                            |

Travaillez en parallèle lorsque c’est utile, puis confrontez vos résultats. Tous les membres doivent participer aux décisions et comprendre la proposition finale. Si une étape dépasse le temps prévu, le SM aide à recentrer le groupe sur les livrables essentiels et consigne ce qui reste à clarifier.

## 9. Remise par le Scrum Master

Complétez le fichier **`DA2M_Rapport_lancement_equipe.md`**, puis :

1. déposez sa version validée par l’équipe dans `docs/` sur GitHub;
2. vérifiez les liens et l’accès de l’enseignante;
3. le SM soumet une seule remise pour l’équipe dans l’espace Teams indiqué, à la fin de la séance.

La remise contient :

- le rapport Markdown;
- le lien du repository appartenant à l’organisation DA2M;
- le lien du GitHub Project appartenant à cette même organisation;
- le nom de l’équipe et l’identité du SM qui soumet.

Le rapport renvoie aux fiches complétées, aux maquettes et aux issues. Les deux liens GitHub doivent ouvrir des espaces déjà créés et consultables.

## 10. Critères de validation de l’activité

Avant la remise, vérifiez ensemble :

- [ ] L’équipe comprend 3 ou 4 membres.
- [ ] Le PO et le SM sont nommés et distincts.
- [ ] Chaque membre possède une première contribution technique précise et une tâche associée.
- [ ] Les règles d’équipe et une première DoD sont écrites.
- [ ] L’idée répond à un problème et à un public identifiés.
- [ ] La fiche d’identité et le persona utilisent les modèles fournis.
- [ ] Les maquettes fournies sont utilisées et les trois pages sont repérées.
- [ ] La navigation, le formulaire et le parcours vers le backend sont décrits.
- [ ] Le dépôt et le Project existent tous deux dans l’organisation DA2M et sont reliés.
- [ ] Le README permet de retrouver le Project et les documents.
- [ ] Le backlog contient au moins 1 Epic, 3 User Stories et 1 tâche par membre, avec les informations demandées.
- [ ] Les liens sont accessibles à l’enseignante.
- [ ] L’équipe a effectué ses propres vérifications et consigné les questions restantes.
- [ ] Le rapport a été relu par tous les membres et soumis par le SM.

**Cette activité est non notée, mais elle est obligatoire et essentielle à la progression du projet.** L’enseignante donnera un retour sur l’idée et l’organisation; les ajustements demandés serviront à poursuivre le travail.

## Références

- [Scrum Guide — responsabilités de l’équipe Scrum](https://scrumguides.org/scrum-guide.html).
- [GitHub — créer un Project](https://docs.github.com/en/issues/planning-and-tracking-with-projects/creating-projects/creating-a-project).
- [GitHub — relier un Project à un dépôt](https://docs.github.com/en/issues/planning-and-tracking-with-projects/managing-your-project/adding-your-project-to-a-repository).
- [GitHub — créer un dépôt](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository).
