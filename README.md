# RENDU-1
# Application de Gestion des Événements et Réservations avec JDBC

Ce projet implemente une application Java permettant de gérer des utilisateurs, des événements, des salles, des terrains, et des reservations via JDBC. L'application interagit avec une base de donnees relationnelle MySQL pour effectuer des operations CRUD (Creer, Lire, Mettre à jour, Supprimer)

## Contexte

L'ecole souhaite automatiser la gestion des événements, la réservation des salles et des terrains, ainsi que la gestion des utilisateurs (etudiant et professeur). Cette application permet de gerer les utilisateurs, les événements et les reservations de maniere simple

## Fonctionnalités

### 1. Gestion des Utilisateurs
- Ajouter un utilisateur
- Afficher la liste des utilisateurs
- Supprimer un utilisateur

### 2. Gestion des Événements
- Ajouter un evenement
- Afficher les evenements
- Modifier un evenement
- Supprimer un evenement

### 3. Gestion des Salles et Terrains
- Ajouter une salle
- Afficher les salles disponibles
- Supprimer une salle
- Ajouter un terrain
- Afficher les terrains disponibles
- Supprimer un terrain

### 4. Gestion des Reservations
- Reserver une salle et/ou un terrain pour un événement
- Verifier la disponibilite d'une salle/terrain
- Afficher les reservations existantes
- Modifier une reservation
- Supprimer une reservation

## Structure de la Base de Donnees

La base de donnees comprend les tables suivantes :

1. **Utilisateurs** : Contient les informations des utilisateurs (etudiant et professeur)
   - id_user, nom, prenom, email, type (étudiant ou professeur)

2. **Evenements** : Contient les informations des événements
   - id_event, nom_event, date_event, description, id_user (référence à l'utilisateur responsable)

3. **Salles** : Contient les informations des salles
   - id_salle, nom_salle, capacite

4. **Terrains** : Contient les informations des terrains.
   - id_terrain, nom_terrain, type

5. **Reservations** : Contient les informations des reservations effectuees
   - id_reservation, id_user, id_event, id_salle, id_terrain, date_reservation


