#  Book Recommender System

Un système intelligent de recommandation de livres utilisant l'apprentissage automatique et le filtrage collaboratif.

##  Description du Projet

Ce projet implémente un système de recommandation de livres basé sur l'apprentissage automatique. En utilisant des techniques de filtrage collaboratif et l'algorithme des k-plus proches voisins (KNN), le système suggère des livres similaires en fonction des préférences des utilisateurs.

##  Fonctionnalités

-  **Recommandations personnalisées** basées sur les similarités entre les livres
-  **Affichage des couvertures** des livres recommandés
-  **Interface utilisateur intuitive** avec Streamlit
-  **Algorithmes ML avancés** utilisant K-Nearest Neighbors
-  **Traitement de données massives** avec optimisation mémoire

##  Technologies Utilisées

- **Python 3.11+**
- **Streamlit** - Interface utilisateur web
- **Scikit-learn** - Algorithmes de machine learning
- **Pandas & NumPy** - Traitement des données
- **SciPy** - Calculs scientifiques et matrices creuses
- **Pickle** - Sérialisation des modèles

##  Structure du Projet
book-recommender-system/
├── artifacts/
│ ├── model.pkl # Modèle ML entraîné
│ ├── books_name.pkl # Noms des livres
│ ├── final_rating.pkl # Données de ratings finales
│ └── book_pivot.pkl # Matrice pivot des livres
├── Data/
│ ├── BX-Books.csv # Données des livres
│ ├── BX-Users.csv # Données des utilisateurs
│ └── BX-Book-Ratings.csv # Données des évaluations
├── Books_Recommender.ipynb # Notebook d'analyse et d'entraînement
├── app.py # Application Streamlit principale
└── README.md # Documentation du projet


## 📊 Dataset

Le projet utilise le **Book-Crossing Dataset** contenant :
- **271,360 livres** avec informations détaillées
- **278,858 utilisateurs** avec données démographiques
- **1,149,780 évaluations** sur une échelle de 0-10

### Prétraitement des Données
- Filtrage des utilisateurs avec plus de 200 évaluations
- Sélection des livres avec au moins 50 évaluations
- Nettoyage et normalisation des données
- Création de matrices creuses pour l'optimisation

##  Installation et Utilisation

### Prérequis
- Python 3.11 ou version supérieure
- pip (gestionnaire de paquets Python)

### Installation

1. **Cloner le repository**
```bash
git clone https://github.com/hajarelkamri/book-recommender-system.git
cd book-recommender-system
2. Créer un environnement virtuel
python -m venv venv
source venv/bin/activate
3. Installer les dépendances
pip install -r requirements.txt
4.Lancer l'application
streamlit run app.py

 Comment Utiliser
Lancez l'application avec streamlit run app.py

Sélectionnez un livre dans le menu déroulant

Cliquez sur "Show Recommendation"

Découvrez 5 livres similaires avec leurs couvertures

 Algorithmes et Méthodologie
Filtrage Collaboratif
Le système utilise le filtrage collaboratif basé sur les similarités entre les utilisateurs et les livres.

K-Nearest Neighbors (KNN)
Algorithme: Brute-force pour les calculs de similarité

Métrique: Distance euclidienne

Voisins: 6 livres les plus similaires
