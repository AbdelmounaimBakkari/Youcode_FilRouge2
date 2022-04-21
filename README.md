# Youcode_FilRouge2 
# ChatChat

## Contexte du projet
En cadre de réaliser projet Fil rouge de fin d’étude après la formation en deuxième année en Youcode, mon projet de Fil rouge est le site ChatChat.

ChatChat est une application simple du monde réel où les utilisateurs peuvent écrire de courts tweets, suivre chacun
Ce projet est idéal pour ceux qui souhaitent approfondir une pile complète à l'aide de Nodejs et MongoDB après avoir appris HTML, CSS et JS. Construire une application full stack à lui tout seul est une tâche difficile, mais apprendre et créer de telles applications vous aidera à maîtriser vos compétences.

Construire ce projet sera une tâche difficile où vous apprendrez et explorerez tous sur le modèle MVC, la base de données NoSQL (MongoDB) et bien plus encore.

## Objective
Créez une application Web complète - ChatChat (une application de médias sociaux) à l'aide de Node.JS, Express.Js, MongoDB, React (MERN Stack)

## Étapes du projet
Nous pouvons diviser le projet en fonction de la pile utilisée :

• ReactJS : création de l'interface utilisateur de l'application

• Familiarisation avec l'environnement NodeJS

• ExpressJS : Framework de création de serveurs.

• MongoDB : Utilisation de la base de données NoSQL.

• GitHub : pour publier votre projet.

## Tâche 1 : Créer le serveur Express
Dans cette tâche, nous allons commencer à utiliser Node.js et Express.js pour créer le backend de l’application. Décomposons cette tâche en quelques étapes :

Création du serveur Web à l'aide d'Express.

Connaître la structure des fichiers et mettre en place le projet.

- [x] Conditions

• Commencez à construire un serveur en utilisant express. Express.js, qui est un framework léger pour la création de serveurs Web, facilite l'organisation des fonctionnalités de votre application avec des middlewares et du routage.

• Après avoir construit le serveur, votre dossier de projet doit être composé du fichier server.js avec package.json, package-lock.json et node_modules.


## Tâche 2 : Utilisation de la base de données MongoDB avec le serveur Express en suivant l'architecture MVC

Dans ce projet, nous utiliserons MongoDB comme base de données. Reportez-vous à ceci pour savoir pourquoi nous devrions préférer NoSQL aux bases de données SQL dans certains cas.

Divisons cette tâche en quelques étapes :

1. Créer un compte atlas MongoDB pour gérer nos données.
2. Connexion de la base de données au serveur express.
3. Connaître l'architecture MVC dans les applications Node.js.
Nous allons maintenant commencer à diviser le projet en un modèle MVC. M qui signifie Model est l'endroit où nous allons inclure toute notre logique métier ou toutes les règles que nous voulons appliquer à nos données. V qui signifie Views, c'est-à-dire l'UI (User Interface). C qui signifie contrôleur est l'intermédiaire en fonction de la demande entrante. Il appellera le modèle approprié avec la logique appropriée.

Une fois cela fait, le contrôleur appellera la vue appropriée et lui transmettra toutes les données dynamiques pertinentes du modèle.

- [x] Conditions

• Créez un compte Atlas. Connectez-vous à votre cluster, insérez et visualisez les données dans votre cluster.

• Créez un fichier db.js dans votre dossier et créez une connexion à une instance MongoDB qui renvoie la référence à la base de données.

• Établissez la connexion de manière à ce que le serveur ne commence à écouter les requêtes qu'une fois la connexion à la base de données établie.

• Explorez l'architecture MVC avant de commencer à implémenter les fonctionnalités dans la tâche suivante.

## Tâche 3 : Mise en œuvre system de l'authentification

Dans cette tâche, nous allons créer l'authentification pour l'application. Divisons cette tâche en étapes plus petites :
1. Création de modèles pour les utilisateurs.
2. Hachage du mot de passe avant de le stocker dans la base de données.
3. Implémentation de l'authentification basée sur la session.
4. Utilisation de Gravatar pour les photos de profil utilisateur.

- [x] Conditions

Implémentez le routage de toutes les routes dans un fichier séparé et appelez les fonctions du contrôleur, respectivement.

• Séparez les contrôleurs et les modèles en fonction de leurs fonctionnalités. Par exemple, créez des fonctions liées à l'utilisateur dans userController.js et des modèles dans userModel.js. Validez les attributs avant de les stocker dans la base de données. Comme ça, divisez les autres en fonction des fonctionnalités. Reportez-vous ceci

• Implémentez le hachage avant de stocker les mots de passe dans la base de données. Pour le hachage, les packages bcryptjs et md5 peuvent être utilisés.

• Vous pouvez également utiliser Mongodb sans Mongoose. Mais l'utilisation de mangouste facilite la mise en œuvre des fonctionnalités.

• Utilisez Session pour l'authentification des utilisateurs.

• Utilisez gravatar pour les photos de profil d'utilisateur.


## Tâche 4 : Implémentation des fonctionnalités de base des utilisateurs

Dans cette tâche, nous allons construire les fonctionnalités de base de l'application. Divisons cette tâche en petites étapes :

1. Construire le modèle pour les postes.
2. Laisser les utilisateurs créer et modifier leurs messages.
3. Laisser les utilisateurs se suivre.
4. Le tableau de bord de l'utilisateur comprendra les messages des autres utilisateurs qu'ils suivent
- [x] Conditions

• Créez un modèle de base de données pour les publications en incluant tous les attributs qui doivent être enregistrés pour la publication.

• Écrivez votre fonction de contrôleur pour enregistrer et modifier les messages par l'utilisateur.

• Construisez le modèle de manière à ce que les followers et les suivis puissent être récupérés par l'utilisateur. (Astuce : utiliser la collection à l'intérieur de la collection, pas de clé étrangère dans la base de données noSQL)

• Récupérez les publications des utilisateurs que vous suivez dans leur tableau de bord respectif.

## Tâche 5 : Construire des pages en utilisant React JS

● Si vous avez parcouru la démo de l'application, vous avez peut-être observé la disposition des pages. Nous pouvons classer le frontend en :

```
  ○ home-guest page 
  ○ home-dashboard page 
  ○ create-post page 
  ○ profile page 
  ○ single post screen page
  ○ header 
  ○ footer
 ```
● Essayez d'inspecter les pages et divisez-les en divisions. Vous pouvez également essayer de créer vos styles CSS pour créer une interface d'application similaire. Ce sera impressionnant si vous venez avec votre propre design.

● Bootstrap joue le rôle le plus important pour construire facilement ces composants.

- [x] Conditions

• Créez l'interface utilisateur de base pour les pages d'invités et le tableau de bord d'accueil (qui s'affichent après la page de destination des formulaires de connexion/inscription initiale). Vous pouvez commencer à utiliser les composants d'amorçage ici même.

• Créez les componetes react en utélise JSX.

• Flexbox joue le rôle le plus important lors de la construction des mises en page.
