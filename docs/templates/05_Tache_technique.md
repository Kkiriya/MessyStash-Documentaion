# Fiche - Tâche technique

> **Une fiche par tâche.** Les Developers définissent, estiment et organisent le travail nécessaire pour réaliser la User Story. Une tâche décrit une action technique précise et un résultat vérifiable.

**Produit et équipe :** [Nom du produit - Nom de l’équipe]
**Identifiant et titre :** [T01 - Verbe d’action et résultat technique]
**User Story concernée :** [Identifiant, titre et lien]
**Parent immédiat :** [User Story, ou tâche parente en cas de découpage]
**Developer(s) qui prennent le travail :** [À renseigner lors de la prise en charge]
**Issue GitHub :** [Lien après création]
**Date et version :** [Date - Version]

## 1. Objectif technique

**Que faut-il réaliser ?**
[Action technique et résultat attendu : écran, service, route, modèle, vérification ou autre.]

**À quelle partie de la User Story cette tâche contribue-t-elle ?**
[Expliquer le lien avec le résultat utilisateur.]

**Critère(s) d’acceptation de la User Story concerné(s) :**
[CA-USxx-xx et explication du lien.]

**Zone principale :** [Frontend / Backend / Données / Test / Configuration / Autre]

## 2. Périmètre et livrable

**Éléments à créer ou modifier :**
[Fichiers, composant, route, données ou document concerné.]

**Entrées ou prérequis :**
[Données, contrat API, maquette, configuration ou autre élément nécessaire.]

**Résultat concret à produire :**
[Ce qui sera disponible et vérifiable à la fin.]

**Règles techniques à respecter :**

- [Format attendu, validation, comportement en erreur ou autre règle pertinente]
- [Autre règle applicable]

**Hors périmètre :** [Travail voisin traité ailleurs, ou Aucun]

## 3. Plan de réalisation

1. [Étape précise]
2. [Étape précise]
3. [Vérification du résultat]

Ces étapes décrivent le travail dans une seule tâche. Créer des issues séparées lorsqu’une partie mérite son propre suivi, sa prise en charge et sa vérification.

## 4. Critères d’acceptation technique / critères de fin

Décrire les conditions concrètes pour terminer cette tâche. Elles couvrent son périmètre technique; la User Story sera ensuite vérifiée comme parcours complet.

| Référence | Condition à satisfaire                                | Vérification et résultat attendu         |
| --------- | ----------------------------------------------------- | ---------------------------------------- |
| CA-T01-01 | [Livrable présent et comportement précis]             | [Comment vérifier et ce que l’on attend] |
| CA-T01-02 | [Cas limite ou erreur pertinent]                      | [Vérification]                           |
| CA-T01-03 | [Intégration ou cohérence avec les autres composants] | [Vérification]                           |

Adapter les critères au travail réel. Pour une tâche de documentation ou de configuration, formuler des vérifications adaptées à ce livrable.

## 5. Poids, priorité et dépendances

**Poids tâche estimé par les Developers :** [1 / 2 / 3 / 5 / 8 selon l’échelle de l’équipe]
**Pourquoi ce poids ?** [Effort, complexité et incertitudes]
**Priorité :** [P1 / P2 / P3; cohérente avec la User Story]
**Dépendances :** [Ce qui doit être disponible avant cette réalisation, ou Aucune]
**Travail pouvant avancer en parallèle :** [Possibilités ou Aucune]

**Question ou obstacle à clarifier :** [Description et prochaine action, ou Aucun]

Le poids est une estimation relative. L’équipe peut réexaminer cette estimation lorsqu’elle comprend mieux le travail.

## 6. Découpage si la tâche est trop grosse

Compléter cette section uniquement si la tâche devient un regroupement de petites tâches. Sinon, indiquer « Aucun découpage nécessaire ».

**Motif du découpage :** [Plusieurs responsabilités, incertitude, volume ou autre raison]
**Poids initial à conserver dans la description :** [Poids avant découpage]

| Petite tâche | Résultat distinct et vérifiable | Poids tâche | Parent | Lien GitHub |
| ------------ | ------------------------------- | ----------- | ------ | ----------- |
| [T01a]       | [Résultat]                      | [Poids]     | [T01]  | [Lien]      |
| [T01b]       | [Résultat]                      | [Poids]     | [T01]  | [Lien]      |

Chaque petite tâche utilise sa propre copie de cette fiche. Relier les petites tâches au parent dans GitHub, ajouter `suivi:parent` au parent et vider son champ Poids tâche dans Projects. Conserver son estimation initiale dans le texte. Les enfants portent les poids du travail à exécuter; leur somme peut différer de l’estimation initiale.

## 7. Métadonnées GitHub

| Élément                       | Valeur à renseigner                                                            |
| ----------------------------- | ------------------------------------------------------------------------------ |
| Label de type                 | `type:task`                                                                    |
| Labels techniques             | [Choisir les labels utiles : frontend, backend, database, test, configuration] |
| Label temporaire de découpage | [a-decouper si nécessaire, sinon Aucun]                                        |
| Label de regroupement         | [suivi:parent après découpage, sinon Aucun]                                    |
| Relation parent               | [User Story ou tâche parente à relier]                                         |
| Project                       | [Nom ou lien]                                                                  |
| Priority                      | [Priorité retenue]                                                             |
| Poids tâche                   | [Estimation; laisser vide pour un regroupement après découpage]                |
| Points US                     | Laisser vide sur une tâche                                                     |
| Assignees                     | [Developer(s) qui prennent le travail]                                         |
| Sprint                        | [Sprint de la User Story après sélection au Planning]                          |
| Status                        | [Backlog / To Do / In Progress / Done]                                         |

Si un obstacle apparaît, ajouter `bloque` et expliquer la cause ainsi que la prochaine action. Le Scrum Master aide l’équipe à traiter les obstacles; les Developers mettent leurs cartes à jour.

## 8. Vérification finale et qualité

**Lien vers la Definition of Done (DoD) commune de l’équipe :** [Lien]

- [ ] Les critères de fin de cette tâche sont vérifiés.
- [ ] Les exigences de qualité applicables de la DoD commune sont satisfaites.
- [ ] Pour une tâche de code, le changement est relu et intégré selon les règles de l’équipe.
- [ ] Les vérifications pertinentes ont réussi; leur résultat est consigné.
- [ ] Les instructions ou documents concernés sont à jour lorsque nécessaire.
- [ ] L’issue, les dépendances et les liens de PR sont à jour.

**PR ou livrable :** [Lien; indiquer sans objet et justifier si nécessaire]
**Vérifications réalisées et résultats :** [Résumé ou liens]
**Points restant à traiter ailleurs :** [Liens vers les issues, ou Aucun]

Terminer une tâche ne suffit pas à terminer sa User Story : celle-ci doit satisfaire ses critères d’acceptation et la DoD sur le résultat complet.
