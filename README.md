Application de Gestion de la Relation Client (CRM) en Qt
Description
Cette application de gestion de la relation client (CRM) est développée en utilisant Qt pour l'interface utilisateur et SQLite pour la base de données. L'application permet de gérer une base de données de contacts et leurs interactions, offrant des fonctionnalités avancées pour l'organisation et la gestion des informations clients.

Fonctionnalités
Gestion des Contacts :

Création de fiches de contact avec les informations suivantes : nom, prénom, entreprise, email, téléphone, photo, date de création.
Modification et suppression de fiches de contact avec horodatage automatique des opérations (création, modification, suppression).
Gestion des Interactions :

Ajout d'interactions (rendez-vous, commentaires) sous forme de champ texte horodaté.
Liste des interactions d'un contact, triées par date de modification.
Système de Tagging :

Utilisation de tags dans les notes des interactions pour les tâches à effectuer et les dates importantes :
@todo pour les tâches à faire.
@date pour les dates importantes.
Base de Données :

Stockage de toutes les informations dans une base de données SQLite.
Recherche de contacts par nom ou entreprise, et par intervalle de dates.
Requêtes pour compter les contacts, les interactions entre deux dates, et collecter les @todo ou @date pour un contact donné et une période donnée.
Exportation :

Exportation des données en format JSON pour l'interopérabilité.
Contraintes et Erreurs à Éviter
Séparation des Structures de Données : Ne pas lier directement les structures de données CRM avec les types Qt pour assurer la généricité des algorithmes.
Utilisation des Conteneurs Standard C++ : Utiliser std::list, std::vector, std::deque, std::map, etc.
Gestion des Erreurs : Vérifier les erreurs lors de la manipulation des données et lors de l'interaction avec l'IHM ou la base de données, et utiliser massivement les exceptions.
Documentation
Les sources C++ sont documentées avec Doxygen. Les commentaires du code permettent la génération d'une documentation complète incluant les classes, les algorithmes et les fonctions. Le diagramme des classes est également généré par Doxygen.
