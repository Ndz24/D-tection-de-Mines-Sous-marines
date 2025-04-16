# Détection de Mines Sous-marines 🌊💣

Ce projet applique l’algorithme des **K plus proches voisins (KNN)** pour identifier si un objet détecté par sonar est une **mine** ou une **roche**. L'objectif est de classer les signaux acoustiques enregistrés en deux catégories : "Mine" (M) ou "Roche" (R).

## 📁 Structure du projet

## 🎯 Objectif
Utiliser un algorithme de classification supervisée pour distinguer les mines sous-marines des roches à partir de signaux sonar.

## 🧰 Technologies utilisées
- Python
- Pandas
- NumPy
- Matplotlib, Seaborn
- Scikit-learn (KNeighborsClassifier, métriques, etc.)

## 📊 Description du dataset (`sonar.all-data.csv`)
- **60 attributs** numériques représentant l’intensité des signaux sonar dans différentes fréquences.
- La **dernière colonne** contient la **classe cible** :
  - `R` pour **Roche**
  - `M` pour **Mine**

Le dataset contient **208 instances**.

## ⚙️ Pipeline du projet
1. Chargement du dataset
2. Analyse exploratoire
3. Encodage des classes (M → 1, R → 0)
4. Séparation des données en jeu d’entraînement et de test
5. Normalisation des données
6. Entraînement du modèle KNN
7. Choix du meilleur **k** (validation croisée)
8. Évaluation : accuracy, matrice de confusion, classification report

## 📈 Résultats
Le modèle KNN fournit de bonnes performances de classification pour la détection de mines avec un choix optimisé de k.
