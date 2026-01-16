# Application de Messagerie — Kaypic Style

Cette application permet aux utilisateurs de communiquer en temps réel à travers des groupes et conversations privées, avec un design inspiré de Microsoft Teams et une palette de couleurs personnalisée.

## Fonctionnalités

### Gestion des groupes
- Création d’un groupe de discussion  
- Rejoindre / quitter un groupe  
- Recherche de groupes et de personnes  
- Fil d’actualité des groupes  

### Messagerie en temps réel
- Envoi et réception de messages instantanés via SignalR  
- Affichage moderne type Teams  
- Système de bulles  
- Historique des messages (stockage BD)

### Partage de fichiers
- Upload fichiers  
- Upload dossiers complets  
- Stockage BD + disque

## Structure BD

### TMessagingPersona
- mp_id (PK)
- ts_id (FK)
- mp_status
- mp_category
- mp_email
- mp_lname
- mp_fname
- created_at

### TMessagingChat
- mc_id (PK)
- ts_id (FK)
- mc_status
- mc_title
- created_by_mp_id
- created_at

## Démonstration

### Vidéo de démonstration (cmd + click)

<a href="https://VanettaLudivine.github.io/WebKaypic/kaypic.mp4" target="_blank">▶ Cliquez ici pour ouvrir la vidéo de démo</a>

*La vidéo montre la navigation complète : connexion → gestion clients → comptes → opérations.*

## Design Kaypic
Couleurs : #5c0010, #9e3b42, #e4717a, #f5abb0, #ffe4ea, #FCF9F9, #F9F8F8, #000000.

## Technologies
ASP.NET Core, SignalR, SQL Server, EF Core, HTML/CSS/JS, Twilio
