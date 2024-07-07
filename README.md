# Système de Recommandation de Films par Paires

Ce projet vise à développer un système de recommandation de films qui suggère deux films complémentaires en fonction des genres, thèmes ou préférences des utilisateurs, similaire au concept utilisé sur [Date Night Movies](https://datenightmovies.com/spider-man-no-way-home+mona-lisa-smile).

## Objectif

L'objectif principal est de construire un système de recommandation utilisant des données provenant des ensembles de données MovieLens et IMDb, en intégrant des informations sur les genres, les métadonnées et les évaluations des films.

## Ensembles de Données

Pour ce projet, nous avons utilisé les ensembles de données suivants :

- **MovieLens Dataset**: [MovieLens](https://grouplens.org/datasets/movielens/)
- **IMDb Dataset**: [IMDb Datasets](https://www.imdb.com/interfaces/)

## Tâches Réalisées

1. **Collecte et Prétraitement des Données**
   - Téléchargement des ensembles de données MovieLens et IMDb.
   - Fusion des ensembles de données pour inclure les évaluations des films, les genres et les métadonnées.

2. **Ingénierie des Fonctionnalités**
   - Extraction des caractéristiques pertinentes telles que les genres, les réalisateurs, la distribution principale et les évaluations des films.
   - Création d'une matrice d'interaction utilisateur-élément pour le filtrage collaboratif.

3. **Développement du Modèle**
   - Implémentation d'un algorithme de système de recommandation (par exemple, la factorisation de matrices) pour prédire la note d'un film par un couple d'utilisateurs.

4. **Algorithme de Recommandation**
   - Développement d'un algorithme pour suggérer un film qui pourrait plaire au couple d'utilisateurs, en utilisant des scores de couple pour chaque film et en triant les films par score.

5. **Évaluation**
   - Division des données en ensembles d'entraînement et de test.
   - Évaluation du modèle en utilisant des métriques choisies.

## Structure des Fichiers

Assurez-vous d'avoir un dossier `datasets` à la racine du projet avec les fichiers suivants :
```
datasets/
├── ml-1m
│   ├── movies.dat
│   ├── ratings.dat
│   └── users.dat
├── name.basics.tsv
├── title.akas.tsv
├── title.basics.tsv
├── title.crew.tsv
├── title.episode.tsv
├── title.principals.tsv
└── title.ratings.tsv
```

## Utilisation du Code

1. **Environnement Virtuel**
   - Créez un environnement virtuel et activez-le :
     ```bash
     python -m venv my_env
     source my_env/bin/activate  # Sur Windows: my_env\Scripts\activate
     ```

2. **Installation des Dépendances**
   - Installez les dépendances nécessaires :
     ```bash
     pip install -r requirements.txt
     ```

3. **Exécution du Notebook**
   - Exécutez le notebook `recommender-system.ipynb` pour revoir le code et les résultats obtenus.

## Résultats et Conclusion

Ce projet fournit une expérience pratique dans la construction d'un système de recommandation réel, intégrant des données provenant de sources multiples. Pour une compréhension détaillée de la méthodologie, des expériences menées, des résultats obtenus et des conclusions tirées, veuillez consulter le rapport PDF complet inclus dans ce repository.