# Corrections  Modélisation d'un Système de Réservation de Vols en Utilisant les Diagrammes de Séquences

## Analyse des Exigences

Imaginons un système de réservation de vols en ligne. Le système permet aux utilisateurs de rechercher des vols, de réserver des billets et de gérer leurs réservations.

## Identification des Scénarios

Les scénarios d'interaction clés sont les suivants :

a. Rechercher un Vol

b. Réserver un Billet

c. Gérer une Réservation

### Scénario 1 : Rechercher un Vol

#### Participants 

Utilisateur, Système de Recherche de Vols

#### Lignes de Vie 

Une ligne de vie pour l'Utilisateur et une ligne de vie pour le Système de Recherche de Vols.

#### Messages 

L'Utilisateur envoie un message "rechercherVol(destination)" au Système de Recherche de Vols. Le Système de Recherche de Vols répond avec un message "listeVols(vols)" contenant la liste des vols disponibles.

### Scénario 2 : Réserver un Billet

#### Participants

Utilisateur, Système de Réservation, Base de Données

#### Lignes de Vie

Une ligne de vie pour l'Utilisateur, une ligne de vie pour le Système de Réservation et une ligne de vie pour la Base de Données.
Messages : L'Utilisateur envoie un message "selectionnerVol(vol)" au Système de Réservation. Le Système de Réservation envoie un message "creerReservation(billet)" à la Base de Données pour enregistrer la réservation.

### Scénario 3 : Gérer une Réservation

#### Participants

Utilisateur, Système de Réservation, Base de Données

#### Lignes de Vie

Une ligne de vie pour l'Utilisateur, une ligne de vie pour le Système de Réservation et une ligne de vie pour la Base de Données.

#### Messages

L'Utilisateur envoie un message "afficherReservations()" au Système de Réservation. Le Système de Réservation envoie un message "recupererReservations(reservations)" à la Base de Données pour obtenir la liste des réservations de l'Utilisateur.

Ces scénarios d'interaction représentent les étapes clés que les utilisateurs effectuent lorsqu'ils interagissent avec le système de réservation de vols en ligne. Chaque scénario implique différents participants, lignes de vie et messages pour montrer comment les interactions se déroulent entre les acteurs et les objets du système.