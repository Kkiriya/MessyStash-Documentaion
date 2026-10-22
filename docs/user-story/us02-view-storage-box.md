# Fiche - User Story

> **Une fiche par User Story.** Le PO clarifie le résultat et sa valeur avec l’équipe. Les Developers discutent la faisabilité, estiment le travail et préparent son découpage. La User Story doit décrire un résultat utile pour l’utilisateur.

> **Exemple de rédaction sommaire :** les règles et propositions ci-dessous sont à valider avec l’équipe avant de considérer la fiche prête.

**Produit et équipe :** MessyStash - Neptune<br>
**Identifiant et titre :** US02 - View Storage Boxes<br>
**Epic parente :** [E01: Manage Storage Box](https://github.com/A26-DA2M/neptune/issues/1)<br>
**Persona et scénario associés :** P01 Alex, scénario 2 organiser une nouvelle boîte de rangement<br>
**Product Owner :** Jean-Simon Cyr<br>
**Issue GitHub :** [Issue](https://github.com/A26-DA2M/neptune/issues/6#event-33164893007)<br>
**Date et version :** 10/13/2026 V1

## 1. Formulation

**En tant que** utilisateur de MessyStash,<br>
**je veux** voir la liste de mes boîtes de rangement,<br>
**afin de** retrouver rapidement une boîte spécifique.

**Pourquoi cette User Story est-elle utile au MVP ?**
Elle permet à Alex de retrouver ses boîtes et d’y accéder pour organiser ses affaires.

## 2. Description et règles

**Situation ou déclencheur :** L’utilisateur veut consulter ses boîtes de rangement.<br>
**Écran(s) ou maquette(s) :** Liste des boîtes. Maquette à venir<br>
**Préconditions :** L’utilisateur a ouvert MessyStash et peut accéder à la gestion des boîtes.

**Règles métier à respecter :**

- La liste affiche les boîtes associées à l’utilisateur.
- Chaque boîte affiche au minimum son nom et sa description.

**Éléments hors périmètre de cette User Story :**
Créer, modifier ou supprimer une boîte, gérer son contenu, définir son emplacement et générer ou lire un code QR. Ces actions pourront être couvertes par d’autres User Stories.

## 3. Critères d’acceptation

Un critère d’acceptation décrit un résultat observable, suffisamment précis pour être vérifié. Préciser les données, l’action et le résultat attendu.

| Référence  | Condition ou action                         | Résultat attendu                                                               | Comment vérifier ?                                                            |
| ---------- | ------------------------------------------- | ------------------------------------------------------------------------------ | ----------------------------------------------------------------------------- |
| CA-US02-01 | L’utilisateur ouvre la liste de ses boîtes. | Ses boîtes s’affichent avec leur nom et leur description.                      | Vérifier que les boîtes affichées correspondent aux données de l’utilisateur. |
| CA-US02-02 | L’utilisateur n’a aucune boîte.             | Un message indique que la liste est vide.                                      | Ouvrir la liste avec un utilisateur sans boîte.                               |
| CA-US02-03 | Le chargement de la liste échoue.           | L’application informe l’utilisateur que les boîtes n’ont pas pu être chargées. | Simuler un échec de chargement et vérifier le message affiché.                |

Adapter le nombre de critères à la fonctionnalité. Lorsqu’une situation est hors périmètre, l’indiquer explicitement plutôt que de laisser son comportement ambigu.

### Scénario d’acceptation - Cas nominal

- **Étant donné** qu’Alex consulte MessyStash,
- **quand** il ouvre la liste de ses boîtes,
- **alors** ses boîtes s’affichent avec leur nom et leur description.

**Critère(s) couvert(s) :** CA-US02-01

### Scénario d’acceptation - Cas limite ou erreur pertinent

- **Étant donné** qu’Alex n’a aucune boîte,
- **quand** il ouvre la liste,
- **alors** un message lui indique que la liste est vide.

**Critère(s) couvert(s) :** CA-US02-02

## 4. Priorité et estimation

**Priorité définie par le PO :** P1 (High)<br>
**Justification de la priorité :** Voir ses boîtes permet à l’utilisateur d’accéder à celle qu’il veut organiser.<br>
**Ordre dans le Product Backlog :** Premier<br>
**Points US estimés par les Developers :** À confirmer<br>
**Hypothèses de l’estimation :** Les boîtes de l’utilisateur sont accessibles depuis une source de données.<br>
**Incertitudes ou dépendances :** Confirmer les renseignements affichés et le comportement en cas de liste vide ou d’échec de chargement.

## 5. Vérification INVEST

INVEST est un repère pour discuter la qualité d’une User Story. Compléter la justification; lorsqu’un point pose problème, préciser l’ajustement envisagé.

| Repère                 | Question à se poser                                                     | Réponse ou ajustement                                                                                                                                                                                                                                             |
| ---------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| I - Indépendante       | Pouvons-nous limiter les dépendances et les chevauchements ?            | Oui, si l’affichage de la liste reste distinct de la création et de la gestion des objets. La liste dépend toutefois d’une source de données qui fournit les boîtes de l’utilisateur; cette dépendance doit être disponible ou simulable pour tester l’affichage. |
| N - Négociable         | Les détails peuvent-ils être clarifiés avec le PO et les utilisateurs ? | Oui. L’ordre des boîtes, les renseignements affichés sur chaque carte et les états vide, chargement et erreur peuvent être définis avec le PO sans changer la valeur principale de la story.                                                                      |
| V - Porteuse de valeur | Quel bénéfice l’utilisateur obtient-il ?                                | L’utilisateur peut repérer rapidement une boîte existante, plutôt que de devoir se souvenir de ses boîtes.                                                                                                                                                        |
| E - Estimable          | Comprenons-nous assez le besoin pour l’estimer ?                        | Oui, si la source de données est disponible et que l’affichage se limite au nom et à la description, avec les états vide et erreur.                                                                                                                               |
| S - Petite             | Peut-elle être terminée dans un Sprint ?                                | Probablement, si le périmètre se limite à récupérer et afficher les boîtes, sans inclure leur création ni la gestion de leur contenu. À confirmer par les Developers.                                                                                             |
| T - Testable           | Les critères permettent-ils de vérifier son résultat ?                  | Oui. Les critères vérifient l’affichage des boîtes, le cas d’une liste vide et l’échec de chargement.                                                                                                                                                             |

## 6. Découpage technique par les Developers

| Tâche | Travail précis                                                                 | Zone                         | Poids tâche | Lien vers l’issue                                                      |
| ----- | ------------------------------------------------------------------------------ | ---------------------------- | ----------- | ---------------------------------------------------------------------- |
| T01   | Programmer une card d'une boite                                                | Frontend                     | Moyen       | [T04](https://github.com/A26-DA2M/neptune/issues/15#event-33759255599) |
| T02   | Chercher l'informations des boîtes dans la base de données                     | Données / Backend / Frontend | Moyen       | [T05](https://github.com/A26-DA2M/neptune/issues/16#event-33759491441) |
| T03   | Vérifier les critères d’acceptation, y compris le comportement en cas d’échec. | Test                         | Moyen       | [T06](https://github.com/A26-DA2M/neptune/issues/17#event-33760282586) |

Adapter les lignes au besoin. La fiche de tâche détaille le travail et sa vérification. Si la User Story reste trop grosse, envisager plusieurs User Stories qui apportent chacune un résultat utile.

## 7. Métadonnées GitHub

| Élément              | Valeur à renseigner                 |
| -------------------- | ----------------------------------- |
| Label de type        | `type:story`                        |
| Autres labels utiles | `feature:boxes`                     |
| Relation parent      | E01 - Manage Storage Box            |
| Project              | Neptune - projet GitHub de l’équipe |
| Priority             | P1 (High)                           |
| Points US            |                                     |
| Poids tâche          | Medium                              |
| Ordre produit        | Deuxième                            |
| Sprint               |                                     |
| Status               | Backlog                             |

## 8. Acceptation fonctionnelle et Definition of Done

Les critères d’acceptation sont propres à cette fonctionnalité. La Definition of Done (DoD) décrit les exigences de qualité communes au produit. Les deux doivent être satisfaits pour considérer cette User Story terminée.

**Lien vers la DoD commune de l’équipe :** À ajouter lorsque la Definition of Done de l’équipe est documentée.

**Vérification de fin :**

- [ ] Tous les critères d’acceptation sont vérifiés et les résultats sont consignés.
- [ ] Le parcours utilisateur complet fonctionne avec les composants réellement nécessaires.
- [ ] Les exigences applicables de la DoD commune sont satisfaites.
- [ ] Les tâches liées et les éventuels ajustements sont à jour dans GitHub.

**Résultats ou preuves :** À compléter après l’implémentation et la vérification (tests, PR ou captures).<br>
**Retours utilisateur ou PO :** À recueillir pendant la validation de la User Story.

Une User Story encore incomplète ne devient pas Done uniquement parce que ses tâches ont été fermées.
