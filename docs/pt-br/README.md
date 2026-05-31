# Predição de Score de Crédito

## Visão Geral

Este é um projeto educacional de ciência de dados para classificação de score de crédito em um cenário fictício. O notebook compara dois modelos e utiliza o modelo com maior acurácia registrada para gerar previsões sobre novos registros.

## Objetivo

Classificar registros nas categorias `Good`, `Standard` e `Poor` usando atributos financeiros e comportamentais disponíveis na base.

## Stack

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn

## Metodologia

1. carregar e inspecionar `clientes.csv`;
2. codificar campos categóricos;
3. separar atributos e variável-alvo;
4. dividir dados de treino e teste;
5. treinar Random Forest e KNN;
6. comparar acurácias;
7. gerar previsões para `novos_clientes.csv`.

## Imagens Explicativas

As imagens originais foram preservadas e agora aparecem com contexto no [relatório final](../../reports/final_report.md).

### Fluxo Simplificado de Treino e Teste

![Exemplo simplificado de treino e teste](../../Imagens%20do%20Projeto/Captura%20de%20tela%20de%202023-09-28%2008-10-04.png)

Esta captura ajuda a distinguir atributos, rótulos esperados e previsões. Ela é uma ilustração conceitual, não um extrato literal da base.

### Intuição do KNN

![Ilustração conceitual do KNN](../../Imagens%20do%20Projeto/modelo_knn%20%281%29.jpg)

A figura representa grupos próximos no espaço de atributos e ajuda a visualizar a ideia de classificação por vizinhança.

### Figura Original de Modelo Baseado em Árvore

A imagem original `modelo_arvore_decisao (1).jpg` foi preservada, mas possui legibilidade visual limitada. O [relatório final](../../reports/final_report.md) registra essa limitação e esclarece que o notebook implementa Random Forest.

## Resultados Registrados

| Modelo implementado | Acurácia registrada no notebook |
| --- | ---: |
| Random Forest | 0.8265 |
| KNN | 0.7350666666666666 |

Os números pertencem à execução salva no notebook. Eles podem variar em uma nova execução porque não há `random_state` fixo.

## Instalação

```bash
python -m venv .venv
python -m pip install -r requirements.txt
```

## Execução Local

Abra `main.ipynb` em um ambiente Jupyter e execute as células na ordem apresentada. Os CSVs originais permanecem na raiz para preservar os caminhos usados no notebook.

## Estrutura

| Caminho | Conteúdo |
| --- | --- |
| `main.ipynb` | Notebook original. |
| `clientes.csv` | Base de treino e teste. |
| `novos_clientes.csv` | Novos registros de exemplo. |
| `Imagens do Projeto/` | Imagens explicativas originais. |
| `reports/final_report.md` | Relatório analítico consolidado. |
| `data/README.md` | Guia dos dados. |

## Limitações e Segurança

Este repositório não é um sistema de decisão de crédito em produção. Consulte [SECURITY.md](../../SECURITY.md), o [relatório](../../reports/final_report.md) e o [roadmap](../../ROADMAP.md).
