# User Story

Follow this template to document **user story**:

```md
# Fiche - User Story

> **Une fiche par User Story.** Le PO clarifie le résultat et sa valeur avec l’équipe. Les Developers discutent la faisabilité, estiment le travail et préparent son découpage. La User Story doit décrire un résultat utile pour l’utilisateur.

**Produit et équipe :** [Nom du produit - Nom de l’équipe]
**Identifiant et titre :** [US01 - Verbe d’action et résultat]
**Epic parente :** [Identifiant, titre et lien]
**Persona et scénario associés :** [Identifiants ou liens]
**Product Owner :** [Nom]
**Issue GitHub :** [Lien après création]
**Date et version :** [Date - Version]

## 1. Formulation

**En tant que** [type d’utilisateur],
**je veux** [action ou possibilité],
**afin de** [bénéfice ou objectif].

**Pourquoi cette User Story est-elle utile au MVP ?**
[Expliquer le lien avec le problème, le persona et l’objectif de produit.]

## 2. Description et règles

**Situation ou déclencheur :** [Quand l’utilisateur a-t-il ce besoin ?]
**Écran(s) ou maquette(s) :** [Liens et éléments concernés]
**Préconditions :** [Situation qui doit déjà être vraie, ou Aucune]

**Règles métier à respecter :**

- [Règle précise, limite, valeur autorisée ou condition]
- [Autre règle pertinente]

**Éléments hors périmètre de cette User Story :**
[Ce qui sera couvert par une autre User Story, ou Aucun.]

## 3. Critères d’acceptation

Un critère d’acceptation décrit un résultat observable, suffisamment précis pour être vérifié. Éviter « le formulaire fonctionne » : préciser les données, l’action et le résultat attendu.

| Référence  | Condition ou action                    | Résultat attendu                      | Comment vérifier ?        |
| ---------- | -------------------------------------- | ------------------------------------- | ------------------------- |
| CA-US01-01 | [Cas nominal : situation et action]    | [Résultat visible ou donnée attendue] | [Essai, test ou parcours] |
| CA-US01-02 | [Règle ou cas limite pertinent]        | [Résultat attendu]                    | [Vérification]            |
| CA-US01-03 | [Erreur ou autre situation pertinente] | [Message et comportement attendus]    | [Vérification]            |

Adapter le nombre de critères à la fonctionnalité. Lorsqu’une situation est hors périmètre, l’indiquer explicitement plutôt que de laisser son comportement ambigu.

### Scénario d’acceptation - Cas nominal

- **Étant donné** [situation initiale et données],
- **quand** [l’utilisateur effectue l’action],
- **alors** [résultat observable attendu].

**Critère(s) couvert(s) :** [Références du tableau]

### Scénario d’acceptation - Cas limite ou erreur pertinent

- **Étant donné** [situation initiale particulière],
- **quand** [action ou événement],
- **alors** [résultat attendu, message et conservation ou modification des données].

**Critère(s) couvert(s) :** [Références du tableau]

## 4. Priorité et estimation

**Priorité définie par le PO :** [P1 haute / P2 normale / P3 basse]
**Justification de la priorité :** [Valeur et ordre logique]
**Ordre dans le Product Backlog :** [Rang décidé par le PO]
**Points US estimés par les Developers :** [1 / 2 / 3 / 5 / 8, selon l’échelle retenue]
**Hypothèses de l’estimation :** [Ce que l’équipe suppose connu ou déjà disponible]
**Incertitudes ou dépendances :** [Références et explications, ou Aucune]

Les points expriment une taille relative; ils ne sont pas une conversion automatique en heures ni la somme obligatoire des poids des tâches.

## 5. Vérification INVEST

INVEST est un repère pour discuter la qualité d’une User Story. Compléter la justification; lorsqu’un point pose problème, préciser l’ajustement envisagé.

| Repère                 | Question à se poser                                                     | Réponse ou ajustement |
| ---------------------- | ----------------------------------------------------------------------- | --------------------- |
| I - Indépendante       | Pouvons-nous limiter les dépendances et les chevauchements ?            | [Réponse]             |
| N - Négociable         | Les détails peuvent-ils être clarifiés avec le PO et les utilisateurs ? | [Réponse]             |
| V - Porteuse de valeur | Quel bénéfice l’utilisateur obtient-il ?                                | [Réponse]             |
| E - Estimable          | Comprenons-nous assez le besoin pour l’estimer ?                        | [Réponse]             |
| S - Petite             | Peut-elle être terminée dans un Sprint ?                                | [Réponse]             |
| T - Testable           | Les critères permettent-ils de vérifier son résultat ?                  | [Réponse]             |

## 6. Découpage technique par les Developers

| Tâche | Travail précis       | Zone                                          | Poids tâche | Lien vers l’issue |
| ----- | -------------------- | --------------------------------------------- | ----------- | ----------------- |
| [T01] | [Travail nécessaire] | [Frontend / Backend / Données / Test / Autre] | [Poids]     | [Lien]            |
| [T02] | [Travail nécessaire] | [Zone]                                        | [Poids]     | [Lien]            |

Adapter les lignes au besoin. La fiche de tâche détaille le travail et sa vérification. Si la User Story reste trop grosse, envisager plusieurs User Stories qui apportent chacune un résultat utile.

## 7. Métadonnées GitHub

| Élément              | Valeur à renseigner                        |
| -------------------- | ------------------------------------------ |
| Label de type        | `type:story`                               |
| Autres labels utiles | [Labels définis par l’équipe]              |
| Relation parent      | [Epic à relier dans GitHub]                |
| Project              | [Nom ou lien]                              |
| Priority             | [Priorité retenue]                         |
| Points US            | [Estimation retenue]                       |
| Poids tâche          | Laisser vide sur la User Story             |
| Ordre produit        | [Rang]                                     |
| Sprint               | [À renseigner après sélection au Planning] |
| Status               | [Backlog / To Do / In Progress / Done]     |

## 8. Acceptation fonctionnelle et Definition of Done

Les critères d’acceptation sont propres à cette fonctionnalité. La Definition of Done (DoD) décrit les exigences de qualité communes au produit. Les deux doivent être satisfaits pour considérer cette User Story terminée.

**Lien vers la DoD commune de l’équipe :** [Lien vers la charte ou le document de référence]

**Vérification de fin :**

- [ ] Tous les critères d’acceptation sont vérifiés et les résultats sont consignés.
- [ ] Le parcours utilisateur complet fonctionne avec les composants réellement nécessaires.
- [ ] Les exigences applicables de la DoD commune sont satisfaites.
- [ ] Les tâches liées et les éventuels ajustements sont à jour dans GitHub.

**Résultats ou preuves :** [Liens vers tests, PR, captures ou compte rendu de vérification]
**Retours utilisateur ou PO :** [Commentaires et suites éventuelles]

Une User Story encore incomplète ne devient pas Done uniquement parce que ses tâches ont été fermées.
```
