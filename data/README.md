# Data Guide

## Current Datasets

The original datasets remain in the repository root to preserve the notebook paths.

| File | Purpose | Rows | Columns |
| --- | --- | ---: | ---: |
| `../clientes.csv` | Training and evaluation data loaded by the notebook. | 100,000 | 25 |
| `../novos_clientes.csv` | Example new records used for predictions. | 3 | 23 |

## Target

The training dataset includes the `score_credito` target column. The notebook describes the possible score categories as `Good`, `Standard`, and `Poor`.

## Features

The notebook removes `id_cliente` and `score_credito` before training. It encodes three categorical fields:

- `profissao`
- `mix_credito`
- `comportamento_pagamento`

## Privacy

Treat customer identifiers and financial attributes as potentially sensitive. Do not replace the educational datasets with real customer exports. Dataset contents were preserved in the documentation-only organization change.
