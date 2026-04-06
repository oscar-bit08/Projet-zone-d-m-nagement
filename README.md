🏠 Projet : Zone Déménagement
Projet scolaire (Spécialité NSI) : Système de recommandation intelligent de quartiers lyonnais basé sur un algorithme de scoring personnalisé.

Réalisé dans le cadre de mes études au Lycée Pierre Brossolette, ce projet permet de croiser des données immobilières et sociales (SQL) avec des algorithmes de pondération (Python) pour aider un utilisateur à choisir son futur lieu de vie.

🛠️ Stack & compétences (sur ce projet)
Langages      → Python · SQL · HTML/CSS · JavaScript

Frameworks    → Flask · Jinja2

Bases         → SQLite (lyon.db)

Outils        → Leaflet.js (Cartographie dynamique) · VS Code

Algorithmique → Programmation Orientée Objet (POO) · Moyennes pondérées

🗂️ Détails du projet
🧠 Logique & Algorithme (Python)
Utilisation de la POO pour structurer les données et le traitement des scores.

Classe Zone : Modélise chaque quartier (ID, Nom, Coordonnées GPS, Budget m², Écoles, Transports...).

Classe Preference : Capture et normalise les critères de l'utilisateur (importance de 0 à 10).

Moteur de Scoring : Algorithme de calcul dynamique qui attribue une note sur 100 à chaque zone en fonction de la distance entre les données réelles et les souhaits de l'utilisateur.

🗄️ Gestion des données (SQL)
Structuration d'une base de données relationnelle pour la métropole lyonnaise.

Création d'une table zones regroupant 35 quartiers (Lyon 1-9, Villeurbanne, Bron, etc.).

Intégration de données socio-économiques : prix moyen au m², densité de crèches, scores de verdure et de commerce.

Script database.sql pour l'initialisation automatisée de l'environnement.

🗺️ Interface & Visualisation
Expérience utilisateur interactive pour rendre les résultats lisibles.

Frontend : Design responsive avec sliders (curseurs) pour ajuster les priorités en temps réel.

Cartographie : Intégration de Leaflet.js pour placer des marqueurs dont la couleur varie selon le score (Vert = Match parfait, Rouge = Éloigné des critères).

Dashboard : Visualisation sous forme de barres de progression des scores détaillés par critère pour chaque quartier proposé.

🖥️ Structure du code
Plaintext
├── app.py              # Serveur Flask, Classes Zone/Preference et Algorithme
├── database.sql        # Script d'injection des données (Lyon & Villeurbanne)
├── lyon.db             # Base de données SQLite générée
├── static/
│   └── style.css       # Design moderne (Gradients, Flexbox, Cards)
└── templates/
    ├── index.html      # Formulaire de saisie des préférences
    └── resultats.html  # Rendu de la carte et du classement des quartiers
📚 Compétences NSI validées
[x] Bases de données : Modélisation et requêtes SQL.

[x] Programmation : Utilisation des classes et méthodes (POO).

[x] Web : Architecture Client-Serveur et protocole HTTP.

[x] Interactivité : Manipulation du DOM et scripts côté client.

📬 Contact
Oscar — Terminale Maths & NSI.
Admis en BTS SIO chez NEXA Lyon, recherche une alternance pour septembre 2026.
