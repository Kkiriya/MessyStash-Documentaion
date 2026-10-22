# Fiche - Persona

Un persona représente un type d’utilisateur et ses besoins. Ses caractéristiques doivent aider à comprendre l’usage du produit.

**Produit et équipe :** MessyStash - Neptune

**Identifiant du persona :** P01

**Auteur(s), date et version :** Émile Valade, 19/10/26, v1

## 1. Portrait

| Élément                                 | Réponse                                                                                                                                                                                                     |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Prénom fictif                           | Alex Tremblau                                                                                                                                                                                               |
| Rôle ou activité                        | Étudiant                                                                                                                                                                                                    |
| Situation pertinente pour le produit    | Alex est un étudiant qui vit en appartement et possède de nombreux objets rangés dans différentes boîtes. Il lui arrive fréquemment d'oublier où il a placé certains objets.                                |
| Aisance avec les outils numériques      | **Niveau :** Intermédiaire à avancé. Alex utilise quotidiennement son téléphone intelligent et son ordinateur pour ses études et ses activités personnelles. Il est à l'aise avec les applications mobiles. |
| Appareil ou environnement d’utilisation | Téléphone intelligent Android, principalement utilisé à domicile lorsqu'il organise ses affaires ou recherche un objet.                                                                                     |

**Photo ou illustration :** ![Portrait d’Alex Tremblau](imgs/P01-pfp.jpg)

**Citation qui résume son besoin :**

> « J'en ai assez de toujours devoir fouiller dans toutes mes boîtes pour retrouver mes affaires ! »

**Origine de cette citation :** phrase fictive représentative

## 2. Objectifs et besoins

**Objectif principal :**

Trouver une meilleure façon d'organiser ses boîtes de rangement afin de retrouver facilement ses objets sans perdre de temps.

| Besoin                                      | Pourquoi ce besoin compte-t-il ?                                                      | Importance pour ce persona |
| ------------------------------------------- | ------------------------------------------------------------------------------------- | -------------------------- |
| B01 - Accès rapide à sa liste d'objets      | Permet de savoir rapidement où se trouve l'objet recherché.                           | Essentiel                  |
| B02 - Interface intuitive et simple         | Alex ne souhaite pas perdre davantage de temps à comprendre une interface compliquée. | Important                  |
| B03 - Organisation des objets par boîte     | Permet de connaître le contenu de chaque boîte sans devoir l'ouvrir.                  | Essentiel                  |
| B04 - Identification des boîtes par code QR | Permet de consulter rapidement le contenu d'une boîte en la scannant.                 | Important                  |

## 3. Frustrations et habitudes actuelles

| Situation ou habitude actuelle                                                  | Difficulté rencontrée                                                           | Conséquence                                                                    |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| Alex range ses objets dans différentes boîtes sans conserver d'inventaire.      | Il oublie dans quelle boîte se trouve un objet.                                 | Il perd du temps à ouvrir et fouiller plusieurs boîtes.                        |
| Lorsqu'il cherche un objet, Alex vérifie manuellement le contenu de ses boîtes. | Certaines boîtes contiennent beaucoup d'objets et sont difficiles à distinguer. | Il doit parfois déplacer plusieurs boîtes avant de retrouver ce qu'il cherche. |
| Alex ajoute régulièrement de nouveaux objets à ses espaces de rangement.        | Il ne possède pas de système pour suivre les changements de contenu.            | Son organisation devient progressivement moins efficace.                       |

**Contraintes d’utilisation :**

Alex souhaite utiliser l'application rapidement, souvent pendant qu'il manipule ses boîtes ou range ses affaires. L'interface doit donc être simple, accessible sur téléphone et permettre de consulter ou d'ajouter des objets en quelques étapes. Une connexion Internet peut être nécessaire selon l'architecture retenue.

## 4. Scénario utilisateur 1

Un scénario raconte une situation complète : un déclencheur, un objectif, une suite d’actions et un résultat. Il prépare les User Stories.

**Titre :** Retrouver un objet rangé dans une boîte

**Situation initiale :** Alex est dans son appartement et souhaite brancher sa console de jeux à son téléviseur.

**Déclencheur :** Il réalise qu'il ne sait plus où il a rangé son câble HDMI parmi ses nombreuses boîtes.

**Objectif :** Retrouver rapidement l'emplacement de son câble HDMI sans devoir ouvrir toutes ses boîtes.

1. Alex ouvre l'application MessyStash sur son téléphone.

2. Il accède à sa liste d'objets et recherche « câble HDMI ».

3. L'application affiche l'objet ainsi que la boîte et la pièce dans lesquelles il est rangé.

4. Alex récupère son câble HDMI à l'emplacement indiqué.

**Résultat attendu et condition de réussite :**

Alex retrouve son câble HDMI grâce aux informations affichées dans l'application. Le scénario est réussi si l'application permet de retrouver l'objet et d'afficher correctement sa boîte et son emplacement.

**Difficulté possible :** L'objet recherché n'a pas été enregistré ou son emplacement n'a pas été mis à jour.

**Besoin de la section 2 concerné :** B01 - Accès rapide à sa liste d'objets.

**Maquette(s) ou écran(s) concerné(s) :** Liste des objets, recherche d'objets et détails d'un objet. Liens à ajouter lorsque les maquettes seront disponibles.

## 5. Scénario utilisateur 2

**Titre :** Organiser une nouvelle boîte de rangement

**Situation initiale :** Alex vient de terminer sa session d'études et souhaite ranger ses anciens cahiers, livres et accessoires scolaires dans une boîte.

**Déclencheur :** Il se rappelle avoir déjà perdu du temps à chercher des objets rangés plusieurs mois auparavant et souhaite éviter que cela se reproduise.

**Objectif :** Enregistrer une nouvelle boîte et son contenu afin de pouvoir retrouver facilement ses objets plus tard.

1. Alex ouvre MessyStash et accède à la gestion de ses boîtes.

2. Il crée une boîte nommée « Matériel scolaire » et indique qu'elle se trouve dans le placard de sa chambre.

3. Il ajoute les objets qu'il souhaite ranger dans cette boîte.

4. Il génère un code QR associé à la boîte afin de pouvoir consulter son contenu en le scannant.

**Résultat attendu et condition de réussite :**

La boîte « Matériel scolaire » apparaît dans la liste des boîtes avec les objets enregistrés. Le scénario est réussi si Alex peut consulter le contenu de sa boîte depuis l'application et retrouver cette boîte à l'aide de son code QR.

**Difficulté possible :** Alex oublie d'ajouter certains objets ou de mettre à jour le contenu de la boîte après avoir déplacé des affaires.

**Besoin de la section 2 concerné :** B03 - Organisation des objets par boîte et B04 - Identification des boîtes par code QR.

**Maquette(s) ou écran(s) concerné(s) :** Liste des boîtes, formulaire de création d'une boîte, formulaire d'ajout d'objet et affichage du code QR. Liens à ajouter lorsque les maquettes seront disponibles.

## 6. Éléments observés et hypothèses

| Information utilisée dans le persona                               | Origine                                                                    | Statut      | Vérification à prévoir                                                            |
| ------------------------------------------------------------------ | -------------------------------------------------------------------------- | ----------- | --------------------------------------------------------------------------------- |
| Les utilisateurs peuvent oublier où ils ont rangé certains objets. | Problématique identifiée par l'équipe lors de la conception de MessyStash. | À confirmer | Interroger des utilisateurs potentiels pour vérifier la fréquence de ce problème. |
| Alex est un étudiant vivant en appartement.                        | Hypothèse de l'équipe pour représenter un utilisateur cible.               | À confirmer | Vérifier si ce profil correspond au public visé.                                  |
| Alex utilise principalement un téléphone Android.                  | Hypothèse de l'équipe.                                                     | À confirmer | Vérifier les appareils utilisés par les utilisateurs potentiels.                  |
| Les utilisateurs souhaitent retrouver rapidement leurs objets.     | Besoin supposé à partir de la problématique du projet.                     | À confirmer | Demander aux utilisateurs comment ils recherchent actuellement leurs objets.      |
| Les codes QR pourraient faciliter l'identification des boîtes.     | Solution envisagée par l'équipe dans le MVP.                               | À confirmer | Faire tester la fonctionnalité à des utilisateurs potentiels.                     |
| Une interface simple est importante pour les utilisateurs.         | Hypothèse de l'équipe.                                                     | À confirmer | Effectuer des tests d'utilisabilité sur les premières maquettes.                  |

Les caractéristiques de ce persona sont principalement basées sur des hypothèses de l'équipe. Elles devront être validées ou ajustées à partir de commentaires et d'observations d'utilisateurs potentiels.

## 7. Liens vers le produit et le backlog

| Besoin ou scénario | Epic concernée        | User Story envisagée ou créée |
| ------------------ | --------------------- | ----------------------------- |
| [Référence]        | [E01 - Titre ou lien] | [US01 - Titre ou lien]        |
| [Référence]        | [Epic]                | [User Story]                  |

Ces liens peuvent être complétés après la rédaction des Epics et des User Stories.

## 8. Critères de validation de cette fiche

- [x] Le persona représente un utilisateur du public visé.

- [x] Il contient une image, un prénom, des objectifs, des frustrations et une citation.

- [x] Les caractéristiques choisies expliquent des besoins ou des contraintes d’utilisation.

- [x] Les deux scénarios ont chacun un objectif et une condition de réussite observable.

- [x] Les scénarios servent à orienter les maquettes et le backlog.

- [x] Les observations et les hypothèses sont distinguées.

- [ ] L’équipe peut expliquer pourquoi ce persona est pertinent pour le MVP.

**Retour de l’équipe ou de la recherche :** À compléter après la validation du persona par les membres de l'équipe et les premiers retours d'utilisateurs.

**Éléments à vérifier ou ajuster :**

- Valider les besoins identifiés auprès d'utilisateurs potentiels.

- Confirmer que le parcours de recherche d'un objet est suffisamment simple.

- Vérifier que la génération et la lecture des codes QR sont intuitives.

- Ajouter les liens vers les maquettes et les issues GitHub.

- Confirmer que l'illustration du persona est bien présente dans le dépôt.

- Ajuster le persona selon les commentaires recueillis.
