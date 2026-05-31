# Relatório Final: Predição de Score de Crédito

## Visão Geral

Este projeto educacional apresenta um fluxo de classificação supervisionada para prever categorias de score de crédito em um contexto fictício. O notebook original é preservado em `main.ipynb`.

## Objetivo

Treinar modelos de machine learning para classificar novos registros nas categorias `Good`, `Standard` e `Poor`, comparando os resultados registrados para dois estimadores.

## Metodologia

1. carregar `clientes.csv` com pandas;
2. verificar a estrutura da base;
3. codificar `profissao`, `mix_credito` e `comportamento_pagamento`;
4. remover `id_cliente` e separar `score_credito` como variável-alvo;
5. separar 70% dos registros para treino e 30% para teste;
6. treinar `RandomForestClassifier` e `KNeighborsClassifier`;
7. comparar as acurácias registradas no notebook;
8. usar o modelo com maior acurácia registrada para prever três novos registros de `novos_clientes.csv`.

## Resultados Registrados

O notebook contém as seguintes acurácias na execução salva:

| Modelo implementado | Acurácia registrada |
| --- | ---: |
| Random Forest | 0.8265 |
| KNN | 0.7350666666666666 |

Na execução salva, Random Forest obteve a maior acurácia. Como o notebook não fixa `random_state`, os valores podem variar em uma nova execução.

## Leitura das Imagens

### 1. Exemplo Conceitual de Treino e Teste

![Exemplo simplificado de treino, teste e previsão](../Imagens%20do%20Projeto/Captura%20de%20tela%20de%202023-09-28%2008-10-04.png)

**Como ler:** a parte superior representa exemplos com atributos em `x` e rótulos em `y`. A parte inferior ilustra dados de teste, valores esperados e previsões. Esta é uma explicação visual simplificada, não uma captura literal das 25 colunas de `clientes.csv`.

### 2. Referência Visual de Modelo Baseado em Árvore

![Referência conceitual de modelo baseado em árvore](../Imagens%20do%20Projeto/modelo_arvore_decisao%20%281%29.jpg)

**Como ler:** este é o ativo original associado à explicação de modelos baseados em árvore. A legibilidade visual atual é limitada. O notebook implementa `RandomForestClassifier`, um conjunto de árvores, e não uma única árvore de decisão.

### 3. Intuição Visual do KNN

![Ilustração conceitual do KNN](../Imagens%20do%20Projeto/modelo_knn%20%281%29.jpg)

**Como ler:** a figura representa grupos próximos em um espaço de atributos. O KNN classifica uma nova observação considerando a proximidade com exemplos conhecidos.

## Limitações

- a divisão treino/teste não fixa `random_state`;
- a execução salva registra acurácia, mas não matriz de confusão ou métricas por classe;
- os codificadores categóricos são ajustados novamente para os novos registros;
- o notebook é educacional e não inclui governança para decisões reais de crédito;
- a figura original de modelo baseado em árvore precisa de uma versão mais legível.

## Próximos Passos

Consulte o [roadmap](../ROADMAP.md). Melhorias analíticas devem ser feitas separadamente para preservar a leitura histórica do notebook original.
