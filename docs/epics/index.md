# Epics

follow this template to document **epics**:

```md
# Fiche - Epic

**Produit et équipe :** [Nom du produit - Nom de l’équipe]
**Identifiant :** [E01, E02, etc.]
**Titre :** [Grand besoin exprimé clairement]
**Product Owner :** [Nom]
**Issue GitHub :** [Lien après création]
**Date et version :** [Date - Version]

## 1. Besoin et valeur

**À qui cette Epic rend-elle service ?**
[Utilisateur(s) et identifiant(s) des personas.]

**Quel grand besoin regroupe-t-elle ?**
[Décrire le besoin ou le problème, plutôt qu’une liste de composants techniques.]

**Quel résultat voulons-nous rendre possible ?**
[Décrire ce que l’utilisateur pourra accomplir une fois ce besoin satisfait.]

**Pourquoi ce résultat est-il utile ?**
[Bénéfice pour l’utilisateur et lien avec la vision du produit.]

**Lien avec l’objectif de produit :** [Référence ou explication courte]
**Scénarios utilisateur concernés :** [Identifiants ou liens]

## 2. Périmètre

**Ce que cette Epic couvre :**

- [Résultat ou capacité inclus]
- [Autre résultat inclus]

**Ce qu’elle ne couvre pas à cette étape :**

- [Besoin voisin ou fonctionnalité reportée]

**Règles ou contraintes importantes :**
[Règles métier qui influencent les User Stories.]

## 3. User Stories proposées

| Identifiant | Résultat utilisateur / titre | Priorité       | Lien vers l’issue     |
| ----------- | ---------------------------- | -------------- | --------------------- |
| [US01]      | [Résultat utile]             | [P1 / P2 / P3] | [Lien après création] |
| [US02]      | [Résultat utile]             | [P1 / P2 / P3] | [Lien après création] |

Adapter le nombre de lignes au besoin. Chaque User Story est développée dans sa propre fiche et reliée à cette Epic dans GitHub.

## 4. Critères d’acceptation de l’Epic

Décrire les résultats observables qui permettront de vérifier que le grand besoin est satisfait. Ces critères seront précisés dans les User Stories; ils ne constituent pas une tâche supplémentaire.

| Référence | Condition de réussite observable | Comment la vérifier ?       | User Stories qui la couvrent |
| --------- | -------------------------------- | --------------------------- | ---------------------------- |
| CA-E01-01 | [Résultat global attendu]        | [Parcours ou démonstration] | [Identifiants]               |
| CA-E01-02 | [Autre résultat pertinent]       | [Vérification]              | [Identifiants]               |

## 5. Priorité, dépendances et questions

**Priorité proposée par le PO :** [P1 haute / P2 normale / P3 basse]
**Justification :** [Valeur, besoin essentiel, dépendance ou raison du report]
**Dépendances avec d’autres besoins :** [Epics ou User Stories liées; indiquer Aucune si pertinent]

| Question ou hypothèse | À clarifier avec qui ? | Prochaine action |
| --------------------- | ---------------------- | ---------------- |
| [Question]            | [Personne ou groupe]   | [Action]         |

## 6. Métadonnées GitHub

| Élément                        | Valeur à renseigner                                          |
| ------------------------------ | ------------------------------------------------------------ |
| Label de type                  | `type:epic`                                                  |
| Autres labels utiles           | [Labels définis par l’équipe, si pertinents]                 |
| Project                        | [Nom ou lien]                                                |
| Priority                       | [P1 / P2 / P3]                                               |
| Points US et Poids tâche       | Laisser vides sur l’Epic                                     |
| Charge indicative, facultative | [Somme des points des User Stories estimées, ou Non estimée] |
| Sprint                         | Laisser vide si l’Epic couvre plusieurs Sprints              |
| Status                         | [Backlog / To Do / In Progress / Done]                       |

La charge indicative est une information dérivée des User Stories. Elle ne s’ajoute pas à leurs points. Les Developers estiment les User Stories; le PO ordonne les besoins.

## 7. Critères de fin de l’Epic

- [ ] Les résultats définis dans les critères d’acceptation sont vérifiés.
- [ ] Les User Stories incluses sont terminées selon la Definition of Done de l’équipe.
- [ ] Le parcours global reste cohérent lorsque les fonctionnalités sont utilisées ensemble.
- [ ] Les fonctionnalités reportées et les questions restantes sont visibles dans le backlog.

**Parcours ou preuve de vérification :** [Lien ou résumé]
**Retour du PO et des parties prenantes :** [À compléter lors de l’inspection du résultat]
```
