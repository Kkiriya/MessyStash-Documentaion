# Fiche - Idée et identité du produit

**Équipe :** Neptune
**Product Owner :** Jean-Simon Cyr
**Date et version :** 19/10/26

## 1. Identité du produit

| Élément                       | Réponse                                            |
| ----------------------------- | -------------------------------------------------- |
| Nom du produit                | MessyStash                                         |
| Description en une phrase     | System de gestion d'inventaire personel.           |
| Signature ou slogan, si utile | Avec **MessyStash** dite au revoir a votre bordel. |
| Type de produit               | Application Mobile                                 |
| Public principal              | propriétaire ou locataire de maison/appartement    |
| Ton du produit                | Simple, Pratique, Organiser, Clair, ...            |

## 2. Le problème à résoudre

**Dans quelle situation le problème apparaît-il ?**
Vous cherchez un objet specifique, disons un veil appareil photo, mais vous ne vous souvenez plus dans quel boites ou dans quelle piece il est, vous cherchez pendant des heures toutes les boites dans votre maison et enfin vous le trouvez.

Avec messyStash Il suffit de chercher le mot cles `appereil photo` et toutes les boites qui contienent un object qui correspond a ce mots cles apparesse et tous les objets sont accompagne de photo... l'appareil photo est donc retrouver en moins de 5 min.

**Que font actuellement les utilisateurs ?**
Pour l'instant la plupart des gens on un tas de boites ou a la limite un label qui indique le contenut general des boites.

**Quelles difficultés rencontrent-ils ?**

- Localiser et Identifie quelle boites contient l'objet chercher
- Permet de mieux organisez son domicile.

**Qu’est-ce que ces difficultés leur coûtent ?**
Temps perdu, oublis l'existence de certains objets, des heure et des heures de recherche.

## 3. Vision et valeur du produit

**Vision du produit :**
Pour les propriétaire ou locataire qui rencontre un manque d'organisation, MessyStash permet de mieux vous organiser et de vous sauvez du temps, grâce à notre systeme d'inventaire personel.

**Bénéfice principal pour l’utilisateur :**
Trouver un objet specifique n'a jamais ete aussi rapide que maintenant.

**Objectif de produit :**
L'equipe veut un systeme de gestion d'inventaire personel fonctionnel, qui integre les codes barres ou code QR, anisi qu'une fonction de recherche dynamique afin de rapidement trouver un objet.

**Comment observerons-nous que le produit répond au besoin ?**

| Résultat attendu              | Indicateur observable                                                                           | Cible ou condition de réussite                                |
| ----------------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| Trouver un objet rapidement   | Temps nécessaire pour retrouver l'emplacement précis d'un objet.                                | L'utilisateur trouve la bonne boîte en moins de deux minutes. |
| Bonne organisation des objets | Proportion d'objets enregistrés dans l'application qui sont correctement rattachés à une boîte. | Tout les objets créés sont attachés à une boîte.              |

Éviter les formulations seules comme « application agréable » ou « facile à utiliser » : préciser l’action que l’utilisateur doit réussir ou le changement attendu.

## 4. Périmètre de la première version - MVP

Le MVP est la première version assez complète pour résoudre le problème principal. Décrire des possibilités pour l’utilisateur, puis identifier ce qui peut attendre.

| Possibilité offerte à l’utilisateur                                                  | Pourquoi est-elle utile ?                                                                | Essentielle au MVP ? |
| ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------- | -------------------- |
| CRUD pour `boite`                                                                    | permet de creer des objet `boite` qui on un emplacement precis ainsi qu'un liste d'objet | [**Oui** / Non]      |
| CRUD pour `objet`                                                                    | permet de creer des objet `objet` qui on une `boite` ainsi qu'une image                  | [**Oui** / Non]      |
| Creation de label a coller sur les boites pour interagir avec a l'aide du smartphone | Interaction intuitive et physique avec le programme                                      | [Oui / **Non**]      |

**Ce que la première version ne prend pas en charge :**

- Recherche rapide et dynamique des objet creer dans l'application
- In-depth Labels creations
- Estimation de la valeur des biens stockes (pour les assurances par example)

**Contraintes connues :**
[Durée du projet, ressources, plateforme ou autre contrainte réellement applicable.]

- Impression des labels, il faut soit choisir un format specifique qui fonctionne avec un label printer specifique, ou on ils va au large et on fait un format a imprimer et laisse libre choix a l'utilisateur de ce qu'il fait avec.

## 5. Utilisateurs, recherche et maquettes

**Fiches personas associées :** [Identifiants et liens vers les 1 à 2 personas]
**Scénarios utilisateur associés :** [Liens ou références aux scénarios de chaque persona]
**Dossier ou outil de maquettes :** [Lien vers Figma, Excalidraw ou l’outil choisi]

Les supports de conception demandent de couvrir au moins trois écrans principaux du MVP. Indiquer lesquels et ce que l’utilisateur y fait.

| Écran principal             | Action ou besoin couvert                                                               | Lien vers la maquette |
| --------------------------- | -------------------------------------------------------------------------------------- | --------------------- |
| Ecran d'acceuil             | Consulter les `boite` creer, bouton pour creer une nouvelle boites, et un nouvel objet | À venir               |
| Ecran de creation de boites | Creer une `boite` et lui attribuer un emplacement                                      | À venir               |
| Ecran de creation d'objet   | Creer un `objet` et lui attribuer une boites                                           | À venir               |

## 6. Première réflexion technique

Cette section est discutée avec les Developers. Elle reste une première proposition à affiner.

| Partie                         | Choix envisagé      | Raison du choix ou question à résoudre |
| ------------------------------ | ------------------- | -------------------------------------- |
| Frontend                       | Flutter             | Requis par le cours                    |
| Backend                        | Express.js + Prisma | Technologie familiaire                 |
| Données et persistance         | Neon PostgreSQL     | Technologie familiaire                 |
| Communication frontend-backend | Express.js API      | Technologie familiaire                 |

## 7. Hypothèses et questions à clarifier

| Hypothèse ou question   | Comment la vérifier ?                 | Prochaine action et personne qui la prend |
| ----------------------- | ------------------------------------- | ----------------------------------------- |
| Comment lire un code QR | Voir sur internet et la documentation | Lecture - Jean-Simon Cyr                  |

## 8. Critères de validation de cette fiche

Ces critères portent sur la clarté de la proposition. Ils ne remplacent pas la validation du besoin auprès des utilisateurs.

- [x] Le nom, le public et la description du produit sont cohérents.
- [x] Le problème est illustré par une situation concrète.
- [x] La vision explique un bénéfice pour l’utilisateur.
- [x] L’objectif de produit et sa condition de réussite sont compréhensibles.
- [x] Le MVP et les éléments reportés sont clairement distingués.
- [ ] Les personas, les scénarios et les maquettes sont reliés à cette vision.
- [ ] Les contraintes et les hypothèses encore non vérifiées sont visibles.
- [ ] Le PO et les Developers peuvent expliquer la même idée avec leurs propres mots.

**Questions encore ouvertes après discussion :** Est-ce qu'on permet plusieurs photos par objets

**Prochaine mise à jour prévue :** Au courant des prochains cours dès qu'on a vu maquettes.
