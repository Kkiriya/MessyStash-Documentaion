# Fiche - User Story

> **Une fiche par User Story.** Le PO clarifie le résultat et sa valeur avec l’équipe. Les Developers discutent la faisabilité, estiment le travail et préparent son découpage. La User Story doit décrire un résultat utile pour l’utilisateur.

> **Exemple de rédaction sommaire :** les règles et propositions ci-dessous sont à valider avec l’équipe avant de considérer la fiche prête.

**Produit et équipe :** MessyStash - Neptune<br>
**Identifiant et titre :** US03 - Edit a Storage Box<br>
**Epic parente :** [E01: Manage Storage Box](https://github.com/A26-DA2M/neptune/issues/1)<br>
**Persona et scénario associés :** P01 Alex, scénario 2 organiser une nouvelle boîte de rangement<br>
**Product Owner :** Jean-Simon Cyr<br>
**Issue GitHub :** À renseigner<br>
**Date et version :** 10/13/2026 V1

## 1. Formulation

**En tant que** utilisateur de MessyStash,<br>
**je veux** modifier le nom et la description d’une boîte et gérer les objets qui y sont associés,<br>
**afin de** garder mes boîtes et leur contenu à jour.

**Pourquoi cette User Story est-elle utile au MVP ?**
Elle permet à Alex de corriger les renseignements d’une boîte et d’adapter son contenu lorsque ses objets changent.

## 2. Description et règles

**Situation ou déclencheur :** L’utilisateur veut mettre à jour une boîte existante ou les objets qui y sont associés.<br>
**Écran(s) ou maquette(s) :** Détails et formulaire de modification d’une boîte. Maquette à venir<br>
**Préconditions :** L’utilisateur a ouvert MessyStash et peut accéder à une boîte existante.

**Règles métier à respecter :**

- Le nom et la description de la boîte sont requis.
- L’utilisateur peut ajouter ou retirer des objets associés à la boîte.
- Les modifications sont enregistrées sur la boîte concernée.

**Éléments hors périmètre de cette User Story :**
Créer ou supprimer une boîte, modifier les renseignements propres aux objets, définir l’emplacement de la boîte et générer ou lire un code QR. Ces actions pourront être couvertes par d’autres User Stories.

## 3. Critères d’acceptation

Un critère d’acceptation décrit un résultat observable, suffisamment précis pour être vérifié. Préciser les données, l’action et le résultat attendu.

| Référence  | Condition ou action                                                                                          | Résultat attendu                                                                          | Comment vérifier ?                                                         |
| ---------- | ------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| CA-US03-01 | L’utilisateur modifie le nom ou la description d’une boîte avec des renseignements valides, puis enregistre. | Les nouveaux renseignements sont enregistrés et affichés sur la boîte.                    | Modifier un champ et vérifier les renseignements après l’enregistrement.   |
| CA-US03-02 | L’utilisateur ajoute ou retire un objet associé à la boîte, puis enregistre.                                 | Le contenu de la boîte reflète les modifications.                                         | Ajouter ou retirer un objet et vérifier le contenu après l’enregistrement. |
| CA-US03-03 | L’utilisateur laisse le nom ou la description vide, ou l’enregistrement échoue.                              | La modification n’est pas enregistrée et l’application informe l’utilisateur du problème. | Essayer un champ requis vide ou simuler un échec d’enregistrement.         |

Adapter le nombre de critères à la fonctionnalité. Lorsqu’une situation est hors périmètre, l’indiquer explicitement plutôt que de laisser son comportement ambigu.

### Scénario d’acceptation - Cas nominal

- **Étant donné** qu’Alex consulte une boîte existante,
- **quand** il modifie son nom et sa description, puis enregistre,
- **alors** les nouveaux renseignements sont affichés sur la boîte.

**Critère(s) couvert(s) :** CA-US03-01

### Scénario d’acceptation - Cas limite ou erreur pertinent

- **Étant donné** qu’Alex modifie une boîte,
- **quand** il efface son nom et tente d’enregistrer,
- **alors** la modification n’est pas enregistrée et un message indique que le nom est requis.

**Critère(s) couvert(s) :** CA-US03-03

## 4. Priorité et estimation

**Priorité définie par le PO :** P1 (High)<br>
**Justification de la priorité :** Modifier une boîte permet de garder ses renseignements et son contenu à jour.<br>
**Ordre dans le Product Backlog :** Troisième<br>
**Points US estimés par les Developers :** À confirmer<br>
**Hypothèses de l’estimation :** La boîte et les objets disponibles sont accessibles depuis une source de données.<br>
**Incertitudes ou dépendances :** Confirmer les règles d’ajout et de retrait des objets et le comportement en cas d’échec d’enregistrement.

## 5. Vérification INVEST

INVEST est un repère pour discuter la qualité d’une User Story. Compléter la justification; lorsqu’un point pose problème, préciser l’ajustement envisagé.

| Repère                 | Question à se poser                                                     | Réponse ou ajustement                                                                                                                                                         |
| ---------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| I - Indépendante       | Pouvons-nous limiter les dépendances et les chevauchements ?            | Cette story dépend de la création et de la consultation des boîtes. Elle reste distincte de la création et de la suppression; la gestion des objets associés est incluse ici. |
| N - Négociable         | Les détails peuvent-ils être clarifiés avec le PO et les utilisateurs ? | Oui. Les règles d’ajout et de retrait des objets peuvent être précisées avec le PO.                                                                                           |
| V - Porteuse de valeur | Quel bénéfice l’utilisateur obtient-il ?                                | L’utilisateur peut garder à jour les renseignements de ses boîtes et les objets qui s’y trouvent.                                                                             |
| E - Estimable          | Comprenons-nous assez le besoin pour l’estimer ?                        | À confirmer après avoir précisé les règles d’ajout et de retrait des objets.                                                                                                  |
| S - Petite             | Peut-elle être terminée dans un Sprint ?                                | À confirmer par les Developers; la modification des renseignements et la gestion des objets doivent rester limitées à une boîte existante.                                    |
| T - Testable           | Les critères permettent-ils de vérifier son résultat ?                  | Oui. Les critères vérifient la modification des renseignements, la mise à jour du contenu et les erreurs d’enregistrement.                                                    |

## 6. Découpage technique par les Developers

| Tâche | Travail précis                                                               | Zone              | Poids tâche | Lien vers l’issue                                                      |
| ----- | ---------------------------------------------------------------------------- | ----------------- | ----------- | ---------------------------------------------------------------------- |
| T07   | Créer le formulaire de modification des renseignements de la boîte.          | Frontend          | À estimer   | [T07](https://github.com/A26-DA2M/neptune/issues/18#event-33763568746) |
| T08   | Enregistrer les changements et les objets associés.                          | Données / Backend | À estimer   | [T08](https://github.com/A26-DA2M/neptune/issues/19#event-33763576147) |
| T09   | Vérifier les critères d’acceptation, y compris les erreurs d’enregistrement. | Test              | À estimer   | [T09](https://github.com/A26-DA2M/neptune/issues/20#event-33763584176) |

Adapter les lignes au besoin. La fiche de tâche détaille le travail et sa vérification. Si la User Story reste trop grosse, envisager plusieurs User Stories qui apportent chacune un résultat utile.

## 7. Métadonnées GitHub

| Élément              | Valeur à renseigner                      |
| -------------------- | ---------------------------------------- |
| Label de type        | `type:story`                             |
| Autres labels utiles | `feature:boxes`                          |
| Relation parent      | E01 - Manage Storage Box                 |
| Project              | Neptune - projet GitHub de l’équipe      |
| Priority             | À confirmer                              |
| Points US            | À confirmer                              |
| Poids tâche          | Laisser vide sur la User Story           |
| Ordre produit        | Troisième                                |
| Sprint               | À renseigner après sélection au Planning |
| Status               | Backlog                                  |

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
