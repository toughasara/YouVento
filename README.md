Contexte du projet
YouCode souhaite dynamiser la vie étudiante en facilitant la création et la gestion de clubs (tech, design, robotique, etc.) et d'événements associés (ateliers, conférences, hackathons). L'objectif est de fournir un outil centralisé pour les administrateurs et les étudiants, permettant de promouvoir les activités, gérer les inscriptions et encourager les collaborations.

​

Objectif

Développer une application web où les administrateurs peuvent gérer les clubs et leurs événements, tandis que les étudiants peuvent explorer les clubs existants, s’y inscrire et consulter le calendrier des activités.

​

​

Fonctionnalités Clés:

Gestion des clubs : Création, édition, suppression et archivage des clubs (nom, description, logo, catégorie).

Gestion des événements : Ajout d'événements liés à un club (date, lieu, description, capacité maximale).

Calendrier interactif : Visualisation des événements à venir.

Tableau de bord étudiant : Liste des clubs/événements auxquels l'étudiant est inscrit.

​

​

Système d'authentification :

Administrateurs : Accès complet à la gestion.

Étudiants : Inscription aux clubs/événements via un compte.

​

​

User Stories:

En tant qu'admin, je peux créer un club en renseignant ses détails et en uploadant un logo.

En tant qu'admin, je peux planifier un événement pour un club (ex: "Atelier IA le 15/10").

En tant qu'admin, je peux archiver un club temporairement (SoftDelete).

En tant qu'étudiant, je peux m'inscrire à un club ou un événement depuis mon compte.

En tant qu'étudiant, je peux consulter un calendrier regroupant tous les événements.

[Bonus] Envoi de notifications par email aux membres lors de la création d'un événement.

​

​

Technologies Requises:

Laravel et Blade pour le templating, JavaScript pour les interactions (calendrier avec FullCalendar.js).

Authentification : Laravel Sanctum ou Laravel UI Auth. Base de données : PostgreSQL avec relations clubs → events (One-to-Many) et events ↔ users (Many-to-Many via registrations). Tables Principales : users, clubs, events, registrations (pour les inscriptions). Upload de fichiers : Stockage des logos de clubs via Laravel Filesystem.
