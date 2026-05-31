# Credit Score Prediction

## Overview

This educational data science project demonstrates credit score classification in a fictional scenario. The original notebook compares Random Forest and KNN, then uses the model with the highest recorded accuracy for example predictions.

## Methodology

1. load and inspect `clientes.csv`;
2. encode categorical fields;
3. split features and target;
4. create training and test partitions;
5. train Random Forest and KNN;
6. compare recorded accuracy;
7. predict scores for `novos_clientes.csv`.

## Existing Images

The original figures are preserved and explained in the [final report](../../reports/final_report.md). The spreadsheet screenshot illustrates training, test labels, and predictions. The KNN image illustrates proximity-based classification. The original tree-based image remains available but has limited visual legibility.

## Recorded Results

| Implemented model | Accuracy saved in the notebook |
| --- | ---: |
| Random Forest | 0.8265 |
| KNN | 0.7350666666666666 |

The values may change when rerunning the notebook because the train/test split does not define `random_state`.

## Setup

```bash
python -m venv .venv
python -m pip install -r requirements.txt
```

Open `main.ipynb` in Jupyter and run the cells in order. Read the [data guide](../../data/README.md), [security notes](../../SECURITY.md), and [roadmap](../../ROADMAP.md).
