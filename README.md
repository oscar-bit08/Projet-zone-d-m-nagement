# 🏠 Projet : Zone Déménagement

> **Projet scolaire (Spécialité NSI)** : Système de recommandation intelligent de quartiers lyonnais basé sur un algorithme de scoring personnalisé.

Ce projet permet à un utilisateur de trouver son quartier idéal dans la métropole lyonnaise en croisant des données réelles (prix au m², infrastructures, transports) avec ses propres priorités (budget, enfants, écologie).

---

## 🛠️ Stack & compétences (sur ce projet)

Langages      → Python 3 · SQL · HTML/CSS · JavaScript
Frameworks    → Flask (Backend) · Jinja2 (Templating)
Bases         → SQLite (lyon.db)
Cartographie  → Leaflet.js (OpenStreetMap)
Concepts      → Programmation Orientée Objet (POO) · Algorithmique de pondération

---

## 🗂️ Détails techniques

### 🧠 Algorithme de Scoring (POO)
L'intelligence du projet repose sur une architecture en classes (visibles dans app.py) :
* Classe Zone : Modélise les données d'un quartier (GPS, prix_m2, scores transport/vert/commerce).
* Classe Preference : Capture les choix de l'utilisateur et calcule les poids normalisés.
* Moteur de calcul : Applique une moyenne pondérée pour attribuer une note finale sur 100 à chaque zone.

### 🗄️ Base de données (SQL)
* Modélisation : Utilisation d'une base SQLite contenant les données de 35 zones de Lyon, Villeurbanne et Bron.
* Initialisation : Le script database.sql permet de générer la base de données lyon.db automatiquement au premier lancement du serveur via une fonction dédiée dans app.py.

### 🗺️ Interface & Carte
* Leaflet.js : Affichage d'une carte interactive avec des marqueurs colorés dynamiquement (Vert/Orange/Rouge) selon le score de compatibilité.
* UI : Formulaire moderne utilisant des sliders pour ajuster l'importance de chaque critère en temps réel.

---

## 📄 Liste des fichiers

* app.py : Serveur Flask, définition des classes et logique de recommandation.
* database.sql : Script SQL pour la création et le remplissage de la base.
* lyon.db : Base de données SQLite générée.
* index.html : Interface de saisie des préférences (Formulaire).
* resultats.html : Affichage de la carte et du classement des quartiers.
* style.css : Design global de l'application (Gradients et mise en page).

---

## ⚙️ Lancement rapide

1. Installer Flask :
   pip install flask

2. Lancer le serveur :
   python app.py

3. Accès : 
   Ouvrir http://localhost:5000 dans votre navigateur.

---

## 📚 Compétences NSI validées

- [x] Bases de données : Modélisation, jointures conceptuelles et requêtes SQL via Python.
- [x] POO : Structuration du code en classes, constructeurs et méthodes.
- [x] Web : Architecture client-serveur, protocoles HTTP (GET/POST) et rendu de templates.

---

## 📬 Contact

> Oscar — Terminale Maths & NSI.
> Admis en BTS SIO chez NEXA Lyon, recherche une alternance pour septembre 2026.

[![GitHub](https://img.shields.io/badge/GitHub-oscar--bit08-181717?logo=github)](https://github.com/oscar-bit08)
