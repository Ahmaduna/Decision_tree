
# Prédiction du Diabète avec un Arbre de Décision

Ce projet vise à prédire la présence de diabète de type 2 chez des patientes à l'aide de données cliniques. L'analyse est basée sur l'algorithme d'arbre de décision.

## Description de la base de données

La base de données utilisée est la célèbre **Pima Indians Diabetes Database** disponible sur [Kaggle](https://www.kaggle.com/uciml/pima-indians-diabetes-database). Elle contient des informations sur des femmes d'origine amérindienne âgées d'au moins 21 ans. Les colonnes incluent : **Pregnancies** : Nombre de grossesses. **Glucose** : Concentration de glucose dans le plasma à jeun. **BloodPressure** : Pression artérielle diastolique. **SkinThickness** : Épaisseur du pli cutané tricipital. **Insulin** : Taux d'insuline sérique de 2 heures. **BMI** : Indice de masse corporelle. **DiabetesPedigreeFunction** : Fonction pedigree du diabète. **Age** : Âge en années. **Outcome** : Variable cible (0 = Non diabétique, 1 = Diabétique).

## Objectif

L'objectif est de développer un modèle de classification qui utilise un arbre de décision pour prédire si une patiente est diabétique ou non, en fonction de ses caractéristiques cliniques.

## Étapes de l'analyse

### 1. Importation et Nettoyage des Données

- Chargement des données à partir d'un fichier CSV.
- Exploration initiale pour comprendre la distribution des variables.
- Traitement des valeurs manquantes et description des données.

### 2. Visualisation des Données

- Histogrammes des variables pour comprendre leur distribution.
- Diagrammes en barres pour la variable cible.
- Boxplots pour analyser la variabilité des données.
- Analyse des corrélations entre les variables.

### 3. Modélisation avec un Arbre de Décision

- Séparation des données en ensembles d'entraînement et de test.
- Construction d'un premier modèle d'arbre de décision.
- Visualisation de l'arbre et importance des variables.
- Évaluation des performances sur les ensembles d'entraînement et de test.

### 4. Optimisation du Modèle

- Optimisation de la profondeur de l'arbre pour éviter le surajustement.
- Utilisation de la validation croisée pour déterminer les paramètres optimaux.
- Évaluation du modèle optimisé et comparaison des performances avec le modèle initial.

### 5. Analyse des Performances

- Évaluation des performances à l'aide de matrices de confusion, de rapports de classification, et de courbes ROC.

## Résultats

- **Exactitude du modèle** : Le modèle optimisé a atteint une précision de 74% sur l'ensemble de test.
- **Variables les plus importantes** : Les variables `Glucose`, `BMI`, et `Age` ont été identifiées comme les plus influentes dans la prédiction.

## Conclusion

L'utilisation d'un arbre de décision pour la prédiction du diabète a permis de construire un modèle performant qui peut être optimisé pour améliorer encore plus sa précision. Ce modèle peut servir de base pour des systèmes de diagnostic automatique dans les soins de santé.

## Exécution

Pour exécuter ce projet :

1. Cloner le dépôt GitHub.
2. Installer les dépendances nécessaires (`matplotlib`, `seaborn`, `pandas`, `numpy`, `scikit-learn`).
3. Exécuter le notebook Jupyter fourni.

