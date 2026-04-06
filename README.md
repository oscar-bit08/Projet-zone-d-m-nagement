🏠 Projet : Zone Déménagement
Projet scolaire (Spécialité NSI) : Application web de recommandation de quartiers lyonnais basée sur un algorithme de scoring personnalisé.

Ce projet a été conçu pour aider les futurs résidents à trouver le secteur idéal à Lyon en croisant des données réelles (prix m², infrastructures, transports) et des préférences utilisateurs pondérées.

🛠️ Stack & Concepts (NSI)
Langages → Python · SQL · HTML/CSS · JavaScript

Frameworks → Flask · Jinja2

Base de données → SQLite (Relationnelle)

Bibliothèques → Leaflet.js (Cartographie) · OS (Gestion fichiers)

🚀 Fonctionnalités clés
🧠 Algorithme de scoring (POO)
L'intelligence du projet repose sur une architecture en Programmation Orientée Objet :

Classe Zone : Modélise les données d'un quartier (écoles, commerces, budget).

Classe Preference : Stocke et normalise les choix de l'utilisateur.

Calculateur : Applique une moyenne pondérée pour générer un score sur 100.

🗺️ Carte Interactive
Intégration de Leaflet.js pour visualiser les résultats.

Marqueurs colorés dynamiques (Vert/Orange/Rouge) selon la pertinence du quartier.

📊 Gestion des données
Base de données SQLite contenant 30+ zones de la métropole lyonnaise.

Script d'initialisation automatique (database.sql) au premier lancement.

📂 Structure du dépôt
Plaintext
├── app.py              # Serveur Flask & Logique algorithmique (Classes POO)
├── database.sql        # Schéma et données (Inserts SQL)
├── lyon.db             # Base de données relationnelle
├── static/
│   └── style.css       # Design moderne et responsive
└── templates/
    ├── index.html      # Formulaire avec Sliders (Saisie)
    └── resultats.html  # Affichage carte et détails des scores
⚙️ Installation
Cloner le dépôt :

Bash
git clone https://github.com/TON_USERNAME/projet-zone-demenagement.git
Installer Flask :

Bash
pip install flask
Lancer l'application :

Bash
python app.py
Accéder à l'interface sur http://localhost:5000

📚 Contexte scolaire
Ce projet valide plusieurs compétences du programme de Terminale NSI au Lycée Pierre Brossolette :

[x] Traiter des données en tables (SQL)

[x] Utiliser des interfaces de programmation (API Leaflet)

[x] Développer une interface utilisateur web

[x] Programmer en utilisant le paradigme objet

📬 Contact
Oscar — Étudiant en Terminale Maths & NSI.

Actuellement en recherche d'une alternance pour un BTS SIO chez NEXA Lyon (Septembre 2026).
