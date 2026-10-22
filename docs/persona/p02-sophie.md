# Fiche - Persona

Un persona représente un type d’utilisateur et ses besoins. Ses caractéristiques doivent aider à comprendre l’usage du produit.

**Produit et équipe :** MessyStash - Neptune

**Identifiant du persona :** P02

**Auteur(s), date et version :** Émile Valade, 19/10/26, v1

## 1. Portrait

| Élément                                 | Réponse                                                                                                                                                                                                  |
| --------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Prénom fictif                           | Sophie Gagnon                                                                                                                                                                                            |
| Rôle ou activité                        | Employée de bureau et parent                                                                                                                                                                             |
| Situation pertinente pour le produit    | Sophie vit avec sa famille dans une maison. Elle range les décorations saisonnières, les souvenirs et divers accessoires dans des boîtes au sous-sol. Elle a du mal à se souvenir du contenu de chacune. |
| Aisance avec les outils numériques      | **Niveau :** Intermédiaire. Sophie utilise quotidiennement son téléphone pour communiquer, gérer son calendrier et faire des achats en ligne. Elle privilégie les applications faciles à comprendre.     |
| Appareil ou environnement d’utilisation | Téléphone intelligent iPhone, utilisé principalement à domicile, notamment au sous-sol et dans les espaces de rangement.                                                                                 |

**Photo ou illustration :** ![alt text](/imgs/P02-pfp.jpg)

**Citation qui résume son besoin :**

> « J’aimerais savoir ce que contiennent mes boîtes sans avoir à toutes les ouvrir. »

**Origine de cette citation :** Phrase fictive représentative

## 2. Objectifs et besoins

**Objectif principal :**

Garder un inventaire clair des objets rangés dans la maison pour les retrouver facilement au moment voulu.

| Besoin                                      | Pourquoi ce besoin compte-t-il ?                                                      | Importance pour ce persona |
| ------------------------------------------- | ------------------------------------------------------------------------------------- | -------------------------- |
| B01 - Consultation du contenu des boîtes    | Évite de déplacer et d’ouvrir plusieurs boîtes pour retrouver un objet.               | Essentiel                  |
| B02 - Identification des boîtes par code QR | Permet d’identifier rapidement une boîte dont elle ne reconnaît pas le contenu.       | Important                  |
| B03 - Mise à jour simple de l’inventaire    | Permet de garder des informations fiables lorsque des objets sont ajoutés ou retirés. | Essentiel                  |
| B04 - Localisation des boîtes               | Permet de savoir dans quelle pièce ou zone de rangement chercher.                     | Important                  |

## 3. Frustrations et habitudes actuelles

| Situation ou habitude actuelle                                  | Difficulté rencontrée                                       | Conséquence                                                  |
| --------------------------------------------------------------- | ----------------------------------------------------------- | ------------------------------------------------------------ |
| Sophie inscrit parfois une description sommaire sur ses boîtes. | Les étiquettes ne reflètent pas toujours le contenu actuel. | Elle doit ouvrir les boîtes pour vérifier ce qui s’y trouve. |
| Elle entrepose des boîtes dans plusieurs espaces de la maison.  | Elle oublie où certaines boîtes ont été déplacées.          | Elle perd du temps à chercher dans différentes pièces.       |
| Elle sort puis range des décorations selon les saisons.         | Elle oublie de mettre à jour son inventaire.                | Les recherches suivantes deviennent moins fiables.           |

**Contraintes d’utilisation :**

Sophie utilise l’application par courtes périodes, parfois avec une seule main pendant qu’elle déplace des boîtes. Elle souhaite des actions simples et des informations lisibles sur son téléphone. La connexion Internet peut être limitée dans certains espaces de rangement.

## 4. Scénario utilisateur 1

Un scénario raconte une situation complète : un déclencheur, un objectif, une suite d’actions et un résultat. Il prépare les User Stories.

**Titre :** Retrouver les décorations d’Halloween

**Situation initiale :** Sophie prépare la décoration de sa maison et se rend au sous-sol pour chercher ses accessoires d’Halloween.

**Déclencheur :** Plusieurs boîtes se ressemblent et elle ne sait plus laquelle contient les décorations recherchées.

**Objectif :** Identifier la bonne boîte sans toutes les ouvrir.

1. Sophie ouvre MessyStash sur son téléphone.
2. Elle consulte la liste des boîtes ou recherche « Halloween » dans les objets enregistrés.
3. Elle repère la boîte correspondante et consulte son emplacement.
4. Elle récupère la boîte dans la zone indiquée.

**Résultat attendu et condition de réussite :**

Sophie identifie la boîte contenant les décorations et retrouve son emplacement. Le scénario est réussi si l’application affiche les objets concernés et la boîte à laquelle ils appartiennent.

**Difficulté possible :** Les décorations ont été déplacées sans que l’inventaire soit mis à jour.

**Besoin de la section 2 concerné :** B01 - Consultation du contenu des boîtes et B04 - Localisation des boîtes.

**Maquette(s) ou écran(s) concerné(s) :** Liste des objets, liste des boîtes et détails d’une boîte. Liens à ajouter lorsque les maquettes seront disponibles.

## 5. Scénario utilisateur 2

**Titre :** Mettre à jour le contenu d’une boîte

**Situation initiale :** Sophie vient de terminer le rangement des décorations et souhaite ajouter de nouveaux accessoires dans une boîte existante.

**Déclencheur :** Elle constate que la liste des objets enregistrés ne correspond plus au contenu réel de la boîte.

**Objectif :** Mettre à jour l’inventaire pour faciliter les recherches futures.

1. Sophie ouvre MessyStash et scanne le code QR de la boîte.
2. Elle consulte la liste des objets associés à cette boîte.
3. Elle ajoute les nouveaux accessoires et retire de la liste les objets qui ne s’y trouvent plus.
4. Elle vérifie que le contenu affiché correspond aux objets rangés.

**Résultat attendu et condition de réussite :**

L’inventaire de la boîte correspond à son contenu réel. Le scénario est réussi si les modifications sont enregistrées et visibles lorsqu’elle consulte à nouveau la boîte.

**Difficulté possible :** Le code QR est abîmé ou ne peut pas être scanné ; Sophie doit alors retrouver la boîte dans la liste.

**Besoin de la section 2 concerné :** B02 - Identification des boîtes par code QR et B03 - Mise à jour simple de l’inventaire.

**Maquette(s) ou écran(s) concerné(s) :** Lecture de code QR, détails d’une boîte et formulaire d’ajout ou de modification d’objet. Liens à ajouter lorsque les maquettes seront disponibles.

## 6. Éléments observés et hypothèses

| Information utilisée dans le persona                                       | Origine                                            | Statut      | Vérification à prévoir                                                   |
| -------------------------------------------------------------------------- | -------------------------------------------------- | ----------- | ------------------------------------------------------------------------ |
| Certaines personnes stockent des objets saisonniers dans plusieurs boîtes. | Hypothèse de l’équipe.                             | À confirmer | Discuter avec des utilisateurs qui disposent d’espaces de rangement.     |
| Sophie utilise principalement un iPhone.                                   | Hypothèse de l’équipe.                             | À confirmer | Vérifier les appareils utilisés par le public visé.                      |
| Les étiquettes manuelles deviennent parfois inexactes.                     | Hypothèse de l’équipe.                             | À confirmer | Demander comment les utilisateurs identifient actuellement leurs boîtes. |
| Les codes QR faciliteraient la consultation des boîtes.                    | Fonctionnalité envisagée dans le MVP.              | À confirmer | Tester le parcours de lecture des codes QR.                              |
| La mise à jour de l’inventaire doit être rapide.                           | Besoin supposé à partir du contexte d’utilisation. | À confirmer | Observer un utilisateur qui ajoute ou retire des objets.                 |

Les caractéristiques de ce persona sont principalement basées sur des hypothèses de l’équipe. Elles devront être validées ou ajustées à partir de commentaires et d’observations d’utilisateurs potentiels.

## 7. Liens vers le produit et le backlog

| Besoin ou scénario | Epic concernée        | User Story envisagée ou créée |
| ------------------ | --------------------- | ----------------------------- |
| [Référence]        | [E01 - Titre ou lien] | [US01 - Titre ou lien]        |
| [Référence]        | [Epic]                | [User Story]                  |

Ces liens peuvent être complétés après la rédaction des Epics et des User Stories.

## 8. Critères de validation de cette fiche

- [x] Le persona représente un utilisateur du public visé.
- [ ] Il contient une image, un prénom, des objectifs, des frustrations et une citation.
- [x] Les caractéristiques choisies expliquent des besoins ou des contraintes d’utilisation.
- [x] Les deux scénarios ont chacun un objectif et une condition de réussite observable.
- [x] Les scénarios servent à orienter les maquettes et le backlog.
- [x] Les observations et les hypothèses sont distinguées.
- [ ] L’équipe peut expliquer pourquoi ce persona est pertinent pour le MVP.

**Retour de l’équipe ou de la recherche :** À compléter après la validation du persona par les membres de l’équipe et les premiers retours d’utilisateurs.

**Éléments à vérifier ou ajuster :**

- Valider les besoins identifiés auprès d’utilisateurs potentiels.
- Vérifier que les parcours de consultation et de modification des boîtes sont simples.
- Tester la lecture des codes QR dans les espaces de rangement.
- Ajouter les liens vers les maquettes et les issues GitHub.
- Ajouter l’illustration du persona au dépôt.
- Ajuster le persona selon les commentaires recueillis.
