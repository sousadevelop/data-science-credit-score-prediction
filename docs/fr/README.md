# Prédiction du Score de Crédit

## Vue d'ensemble

Ce projet pédagogique de science des données présente une classification du score de crédit dans un scénario fictif. Le notebook d'origine compare Random Forest et KNN, puis utilise le modèle ayant la meilleure précision enregistrée pour produire des prédictions d'exemple.

## Méthodologie

1. charger et inspecter `clientes.csv` ;
2. encoder les champs catégoriels ;
3. séparer les attributs et la cible ;
4. créer les partitions d'entraînement et de test ;
5. entraîner Random Forest et KNN ;
6. comparer les précisions enregistrées ;
7. prédire les scores pour `novos_clientes.csv`.

## Images Existantes

Les figures d'origine sont conservées et expliquées dans le [rapport final](../../reports/final_report.md). La capture du tableur illustre l'entraînement, les étiquettes de test et les prédictions. L'image KNN illustre la classification par proximité. L'image d'origine associée aux arbres reste disponible, mais sa lisibilité visuelle est limitée.

## Résultats Enregistrés

| Modèle implémenté | Précision enregistrée dans le notebook |
| --- | ---: |
| Random Forest | 0.8265 |
| KNN | 0.7350666666666666 |

Les valeurs peuvent varier lors d'une nouvelle exécution, car la séparation entraînement/test ne définit pas `random_state`.

## Installation

```bash
python -m venv .venv
python -m pip install -r requirements.txt
```

Ouvrez `main.ipynb` dans Jupyter et exécutez les cellules dans l'ordre. Consultez le [guide des données](../../data/README.md), les [notes de sécurité](../../SECURITY.md) et la [roadmap](../../ROADMAP.md).
