# 📊 Exploring Predictive Health Factors: PCOS Lifestyle Impact Analysis

## 📝 Description du Projet
Ce projet s'inscrit dans le cadre de la compétition **Kaggle Polycystic Ovary Syndrome (PCOS) Lifestyle Impact Research Competition**, organisé par le Kaggle Master yunsuxiaozi, dont l'objectif est d'analyser l'impact des choix de style de vie sur le **syndrome des ovaires polykystiques (SOPK)**. Le SOPK est un trouble endocrinien courant qui affecte la santé reproductive et la qualité de vie des femmes. Ce projet vise à explorer les facteurs prédictifs de la santé reproductive en utilisant des techniques avancées de **machine learning** et d'analyse de données.

Le dataset utilisé a été généré à partir d'un modèle de deep learning entraîné sur des données réelles de SOPK. Les distributions des caractéristiques sont proches de l'original, mais pas identiques, ce qui permet d'explorer les différences et d'améliorer les performances des modèles.



## 🎯 Objectifs

- **Exploration des données** : Analyser les tendances, les corrélations et les patterns dans les données liées au SOPK.
- **Prédiction du SOPK** : Construire des modèles de **machine learning** pour prédire la présence de SOPK en fonction des facteurs de style de vie.
- **Optimisation des modèles** : Utiliser des techniques d'optimisation pour maximiser les performances des modèles.
- **Gestion du déséquilibre des classes** : Appliquer des techniques comme **SMOTE** pour équilibrer les classes de la variable cible.



## 🛠️ Fonctionnalités Implémentées

### 1️⃣ Prétraitement des Données
- Gestion des valeurs manquantes avec **IterativeImputer**.
- Catégorisation des variables (*âge, type d'exercice*).
- Gestion des **outliers** avec les méthodes **IQR et Z-score**.
- Encodage des variables catégorielles avec **LabelEncoder**.

### 2️⃣ Ingénierie des Caractéristiques
- Création de nouvelles variables interactives (*ex : interaction entre le sommeil et l'exercice*).
- Calcul de l'**IMC** et d'autres ratios pour capturer des relations complexes.
- Transformation des variables numériques (**logarithmique, exponentielle, carrée**).

### 3️⃣ Modélisation
- Entraînement de plusieurs modèles de **machine learning** (*Logistic Regression, Random Forest, XGBoost, LightGBM, etc.*).
- Utilisation de la **validation croisée (KFold)** pour évaluer les performances des modèles.
- Sélection du **meilleur modèle** basé sur la métrique **AUC-ROC**.

### 4️⃣ Optimisation des Hyperparamètres
- Utilisation de **Optuna** pour optimiser les hyperparamètres des modèles.
- Maximisation de la métrique **AUC-ROC**.

### 5️⃣ Gestion du Déséquilibre des Classes
- Application de la technique **SMOTE** pour équilibrer les classes de la variable cible (**PCOS**).

### 6️⃣ Évaluation et Prédiction
- Visualisation des **courbes ROC** et des **matrices de confusion**.
- Génération des **prédictions** sur l'ensemble de test et création d'un fichier de soumission pour la compétition.



## 📊 Résultats

- **AUC-ROC** : Le meilleur modèle atteint une performance de **0.78** sur l'ensemble de validation après optimisation.
- **Matrice de Confusion** : Visualisation des performances du modèle en termes de **précision, rappel et F1-score**.


