# Fiche - Epic

**Produit et équipe :** MessyStash, Neptune
**Identifiant :** E01
**Titre :** Gestion des boites
**Product Owner :** Jean-Simon Cyr
**Issue GitHub :** [Lien après création]
**Date et version :** 19/10/26, v1

## 1. Besoin et valeur

**À qui cette Epic rend-elle service ?**
Aux utilisateurs qui souhaitent organiser leurs espaces de rangement, notamment Alex Tremblau (P01) et Sophie Gagnon (P02).

**Quel grand besoin regroupe-t-elle ?**
Les utilisateurs possèdent plusieurs boîtes de rangement et peuvent avoir de la difficulté à se rappeler leur emplacement ou à les distinguer. Ils ont besoin d'un moyen simple de répertorier et de gérer leurs boîtes.

**Quel résultat voulons-nous rendre possible ?**
Permettre aux utilisateurs de créer, consulter, modifier et supprimer leurs boîtes de rangement afin de maintenir une organisation claire et à jour.

**Pourquoi ce résultat est-il utile ?**
Une meilleure gestion des boîtes permet de réduire le temps consacré à la recherche d'objets et facilite l'organisation des espaces de rangement. Cette fonctionnalité constitue également la base de la gestion des objets dans MessyStash.

**Lien avec l’objectif de produit :** Faciliter l'organisation et la localisation des objets personnels grâce à un inventaire numérique structuré par boîtes.
**Scénarios utilisateur concernés :**

- P01 - Scénario 2 (Organiser une nouvelle boîte de rangement).
- P02 - Scénarios liés à l'organisation des espaces de rangement, à confirmer.

## 2. Périmètre

**Ce que cette Epic couvre :**

- Créer une boîte de rangement avec un nom et un emplacement.
- Consulter la liste des boîtes enregistrées.
- Consulter les informations d'une boîte.
- Modifier le nom ou l'emplacement d'une boîte.
- Supprimer une boîte devenue inutile.

**Ce qu’elle ne couvre pas à cette étape :**

- La gestion des objets contenus dans les boîtes (Epic distincte).
- La génération et la lecture des codes QR (Epic distincte).
- L'estimation de la valeur des objets et l'optimisation du rangement (fonctionnalités futures).

**Règles ou contraintes importantes :**

- Chaque boîte doit posséder un nom.
- Chaque boîte doit pouvoir être identifiée individuellement.
- Les informations d'une boîte doivent pouvoir être modifiées après sa création.
- Une confirmation doit être demandée avant la suppression d'une boîte.
- Le comportement de suppression d'une boîte contenant des objets doit être défini avant l'implémentation.
- Les informations enregistrées doivent être conservées entre les utilisations de l'application.

## 3. User Stories proposées

| Identifiant | Résultat utilisateur / titre                         | Priorité | Lien vers l’issue     |
| ----------- | ---------------------------------------------------- | -------- | --------------------- |
| US01        | Créer une boîte de rangement                         | P1       | [Lien après création] |
| US02        | Consulter la liste et les informations de mes boîtes | P1       | [Lien après création] |
| US03        | Modifier les informations d'une boîte                | P1       | [Lien après création] |
| US04        | Supprimer une boîte de rangement                     | P2       | [Lien après création] |

Adapter le nombre de lignes au besoin. Chaque User Story est développée dans sa propre fiche et reliée à cette Epic dans GitHub.

## 4. Critères d’acceptation de l’Epic

Décrire les résultats observables qui permettront de vérifier que le grand besoin est satisfait. Ces critères seront précisés dans les User Stories; ils ne constituent pas une tâche supplémentaire.

| Référence | Condition de réussite observable                                                                   | Comment la vérifier ?                                                                     | User Stories qui la couvrent |
| --------- | -------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ---------------------------- |
| CA-E01-01 | L'utilisateur peut créer une boîte et la retrouver dans sa liste.                                  | Créer une boîte et vérifier son apparition dans la liste.                                 | US01, US02                   |
| CA-E01-02 | L'utilisateur peut consulter le nom et l'emplacement d'une boîte.                                  | Ouvrir une boîte existante et vérifier les informations affichées.                        | US02                         |
| CA-E01-03 | L'utilisateur peut modifier les informations d'une boîte et retrouver les nouvelles valeurs.       | Modifier le nom ou l'emplacement d'une boîte, enregistrer et consulter les modifications. | US03                         |
| CA-E01-04 | L'utilisateur peut supprimer une boîte après confirmation.                                         | Supprimer une boîte vide et vérifier qu'elle n'apparaît plus dans la liste.               | US04                         |
| CA-E01-05 | Les boîtes enregistrées restent disponibles après la fermeture et la réouverture de l'application. | Créer une boîte, fermer l'application, la rouvrir et vérifier sa présence.                | US01, US02                   |

## 5. Priorité, dépendances et questions

**Priorité proposée par le PO :** P1 haute (proposition à valider par le PO).
**Justification :** La gestion des boîtes est une fonctionnalité essentielle du MVP. Elle constitue la base de l'organisation des objets et permet de développer les fonctionnalités de localisation et d'identification par code QR.
**Dépendances avec d’autres besoins :**

- E02 - Gestion des objets : les objets doivent pouvoir être associés à une boîte existante.
- E03 - Gestion des codes QR : chaque code QR doit être associé à une boîte identifiable.

| Question ou hypothèse                                                   | À clarifier avec qui ?  | Prochaine action                                               |
| ----------------------------------------------------------------------- | ----------------------- | -------------------------------------------------------------- |
| Une boîte peut-elle exister sans emplacement défini ?                   | Product Owner           | Définir les champs obligatoires lors de la création.           |
| Que se passe-t-il lorsqu'une boîte contenant des objets est supprimée ? | Product Owner et équipe | Définir le comportement attendu et les critères d'acceptation. |
| Plusieurs boîtes peuvent-elles porter le même nom ?                     | Product Owner           | Déterminer les règles d'identification des boîtes.             |
| Comment les données seront-elles conservées ?                           | Équipe de développement | Choisir une solution de persistance adaptée à l'application.   |

## 6. Métadonnées GitHub

| Élément                        | Valeur à renseigner                             |
| ------------------------------ | ----------------------------------------------- |
| Label de type                  | `type:epic`                                     |
| Autres labels utiles           | `feature:boxes`, si adopté par l'équipe         |
| Project                        | [Nom ou lien]                                   |
| Priority                       | P1                                              |
| Points US et Poids tâche       | Laisser vides sur l’Epic                        |
| Charge indicative, facultative | Non estimée                                     |
| Sprint                         | Laisser vide si l’Epic couvre plusieurs Sprints |
| Status                         | Backlog                                         |

La charge indicative est une information dérivée des User Stories. Elle ne s’ajoute pas à leurs points. Les Developers estiment les User Stories; le PO ordonne les besoins.

## 7. Critères de fin de l’Epic

- [ ] Les résultats définis dans les critères d’acceptation sont vérifiés.
- [ ] Les User Stories incluses sont terminées selon la Definition of Done de l’équipe.
- [ ] Le parcours global reste cohérent lorsque les fonctionnalités sont utilisées ensemble.
- [ ] Les fonctionnalités reportées et les questions restantes sont visibles dans le backlog.

**Parcours ou preuve de vérification :** [Lien ou résumé]
**Retour du PO et des parties prenantes :** [À compléter lors de l’inspection du résultat]
