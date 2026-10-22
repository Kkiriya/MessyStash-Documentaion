# Fiche - User Story

> **Une fiche par User Story.** Le PO clarifie le résultat et sa valeur avec l’équipe. Les Developers discutent la faisabilité, estiment le travail et préparent son découpage. La User Story doit décrire un résultat utile pour l’utilisateur.

> **Exemple de rédaction sommaire :** les règles et propositions ci-dessous sont à valider avec l’équipe avant de considérer la fiche prête.

**Produit et équipe :** MessyStash - Neptune<br>
**Identifiant et titre :** US01 - Create a Storage Box<br>
**Epic parente :** [E01: Manage Storage Box](https://github.com/A26-DA2M/neptune/issues/1)<br>
**Persona et scénario associés :** P01 Alex, scénario 2 organiser une nouvelle boîte de rangement<br>
**Product Owner :** Jean-Simon Cyr<br>
**Issue GitHub :** [Issue](https://github.com/orgs/A26-DA2M/projects/4?pane=issue&itemId=270624966&issue=A26-DA2M%7Cneptune%7C5)<br>
**Date et version :** 10/13/2026 V1

## 1. Formulation

**En tant que** utilisateur de MessyStash,<br>
**je veux** créer une boîte de rangement en lui donnant un nom et une description,<br>
**afin de** commencer à organiser mes objets et de les retrouver plus facilement.

**Pourquoi cette User Story est-elle utile au MVP ?**
Elle permet à Alex de créer un espace identifiable pour organiser ses affaires au lieu de dépendre de sa mémoire.

## 2. Description et règles

**Situation ou déclencheur :** L’utilisateur veut commencer à organiser des objets qui seront rangés ensemble.<br>
**Écran(s) ou maquette(s) :** Liste des boîtes et formulaire de création d’une boîte. Maquette à venir<br>
**Préconditions :** L’utilisateur a ouvert MessyStash et peut accéder à la gestion des boîtes.

**Règles métier à respecter :**

- Le nom et la description sont nécéssaire.
- La boîte créée est associée à l’utilisateur qui l’a créée (Si on fait des users).

**Éléments hors périmètre de cette User Story :**
Ajouter ou retirer des objets, modifier ou supprimer une boîte, définir son emplacement et générer ou lire un code QR. Ces actions pourront être couvertes par d’autres User Stories.

## 3. Critères d’acceptation

Un critère d’acceptation décrit un résultat observable, suffisamment précis pour être vérifié. Éviter « le formulaire fonctionne » : préciser les données, l’action et le résultat attendu.

| Référence  | Condition ou action                                                                | Résultat attendu                                                                                                          | Comment vérifier ?                                                                             |
| ---------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| CA-US01-01 | L’utilisateur saisit un nom et une description valides, puis confirme la création. | La boîte est enregistrée et apparaît dans sa liste avec le nom et la description saisis.                                  | Créer une boîte et vérifier son affichage dans la liste.                                       |
| CA-US01-02 | L’utilisateur tente de créer une boîte sans nom ou sans description.               | La boîte n’est pas créée et l’application indique quel champ requis doit être rempli.                                     | Essayer chaque champ requis vide et vérifier le message ainsi que l’absence de nouvelle boîte. |
| CA-US01-03 | L’enregistrement échoue.                                                           | L’application informe l’utilisateur que la boîte n’a pas pu être créée; aucune boîte incomplète n’apparaît dans la liste. | Simuler ou provoquer un échec d’enregistrement et vérifier le message et la liste.             |

Adapter le nombre de critères à la fonctionnalité. Lorsqu’une situation est hors périmètre, l’indiquer explicitement plutôt que de laisser son comportement ambigu.

### Scénario d’acceptation - Cas nominal

- **Étant donné** qu’Alex est dans la liste de ses boîtes,
- **quand** il crée une boîte nommée Matériel scolaire avec une description,
- **alors** la boîte est enregistrée et apparaît dans sa liste avec les renseignements saisis.

**Critère(s) couvert(s) :** CA-US01-01

### Scénario d’acceptation - Cas limite ou erreur pertinent

- **Étant donné** qu’Alex est sur le formulaire de création,
- **quand** il confirme sans saisir de nom,
- **alors** la boîte n’est pas créée et un message lui indique que le nom est requis.

**Critère(s) couvert(s) :** CA-US01-02

## 4. Priorité et estimation

**Priorité définie par le PO :** P1 (High)<br>
**Justification de la priorité :** La création d’une boîte est nécessaire avant de pouvoir y organiser des objets.<br>
**Ordre dans le Product Backlog :** Premier<br>
**Points US estimés par les Developers :** À confirmer<br>
**Hypothèses de l’estimation :** Le formulaire et l’enregistrement d’une boîte peuvent être réalisés sans QR, emplacement ni gestion des objets.<br>
**Incertitudes ou dépendances :** Confirmer les champs obligatoires et vérifier les dépendances avec les choix d’architecture et de stockage des données.

## 5. Vérification INVEST

INVEST est un repère pour discuter la qualité d’une User Story. Compléter la justification; lorsqu’un point pose problème, préciser l’ajustement envisagé.

| Repère                 | Question à se poser                                                     | Réponse ou ajustement                                                                                                 |
| ---------------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| I - Indépendante       | Pouvons-nous limiter les dépendances et les chevauchements ?            | Oui, si la création simple d’une boîte ne dépend pas de l’ajout d’objets ou du QR.                                    |
| N - Négociable         | Les détails peuvent-ils être clarifiés avec le PO et les utilisateurs ? | Oui le caractère obligatoire de la description reste à confirmer.                                                     |
| V - Porteuse de valeur | Quel bénéfice l’utilisateur obtient-il ?                                | L’utilisateur peut commencer à regrouper et organiser ses objets.                                                     |
| E - Estimable          | Comprenons-nous assez le besoin pour l’estimer ?                        | Presque clarifier les champs requis et le comportement en cas d’échec avant l’estimation.                             |
| S - Petite             | Peut-elle être terminée dans un Sprint ?                                | Semble assez petite si le périmètre reste limité au formulaire et à l’enregistrement; à confirmer par les Developers. |
| T - Testable           | Les critères permettent-ils de vérifier son résultat ?                  | Oui la création, la validation des champs et l’échec d’enregistrement ont des résultats vérifiables.                  |

## 6. Découpage technique par les Developers

| Tâche | Travail précis                                                                 | Zone                         | Poids tâche | Lien vers l’issue                                                      |
| ----- | ------------------------------------------------------------------------------ | ---------------------------- | ----------- | ---------------------------------------------------------------------- |
| T01   | Créer le formulaire et afficher les erreurs de validation des champs requis.   | Frontend                     | Moyen       | [T01](https://github.com/A26-DA2M/neptune/issues/12#event-33701553996) |
| T02   | Enregistrer la boîte et la rendre visible dans la liste de l’utilisateur.      | Données / Backend / Frontend | Moyen       | [T02](https://github.com/A26-DA2M/neptune/issues/13#event-33701753573) |
| T03   | Vérifier les critères d’acceptation, y compris le comportement en cas d’échec. | Test                         | Moyen       | [T03](https://github.com/A26-DA2M/neptune/issues/14#event-33702016300) |

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
| Ordre produit        | Premier                             |
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
