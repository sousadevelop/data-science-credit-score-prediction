# data-science-credit-score-prediction
Análise de dados preditiva feita com modelos de IA em Python para determinar o score de clientes como bons ou maus pagadores para uma empresa fictícia.

```markdown
# Projeto de Análise Preditiva usando IA com Python

Este projeto visa analisar de forma preditiva os dados de um data frame em arquivo ".csv", isto é,
usar um processo de identificar a probabilidade de resultados futuros por meio dos dados atuais
com o uso de modelos de Inteligência Artificial, a fim de definir se deteminados clientes de uma empresa fictícia
são bons ou maus pagadores.
> Exemplo muito usado por empresas de crédito

## Instalação das dependências

Caso use o Jupyter para realizar a análise você precisará instalar as dependências da seguinte forma:

!pip install scikit-learn
!pip install numpy
!pip install pandas

Caso não utilize o Jupyter instale elas sem a exclamação na frente (!).
```
---
## Para usar o código do projeto como base para outras analises
1. Baixe as dependências para executar o código da análise
   - Outras dependências são usadas a medida que a análise é feita, por isso, leia o código da análise feita
     para saber quais foram todas as bibliotecas usadas.
3. Leia os comentários do projeto para entender como é feita a análise
4. Siga os 5 passos princípais de toda análise descritiva, que são:
   - Passo 1: Importar a base de dados
   - Passo 2: Preparar a base de dados para a IA
   - Passo 3: Criar um modelo de IA -> Score crédito: Good(Bom), Standard(Médio), Poor(Ruim)
   - Passo 4: Escolher o melhor modelo de IA
   - Passo 5: Fazer novas previsões
5. Mude o *read_csv()* para o tipo de arquivo que irá analisar, assim como o próprio arquivo que está entre aspas(").
---
## A imagem abaixo mostra um exemplo de como os dados podem ser extraídos e analisados
![image](https://github.com/sousadevelop/Predictive_Score_Analysis/assets/92130316/f73d7cf9-9227-4914-83f3-e680bdb906da)


**Para uma visão mais detalhada você poderá ver no arquivo acima:** *main.ipynb*
---
## Sobre os modelos de Inteligência Artificial usados neste projeto
```
Modelo Árvore de Decisão

    Ele cria uma "árvore" onde faz questões sobre um dado e com base na resposta (sempre sim ou não) ele segmenta os dados.

Modelo KNN -> nearest neighbors - vizinhos mais próximos

    Ele pega uma referência de cada segmento dos dados e julga todos os demais ao redor pela proximidade que possuem da referência,
    ou seja, se uma pessoa tem o score ruim, todos próximos dele serão julgados com o score ruim.
```

[Modelo Árvore de Decisão]
![modelo_arvore_decisao](https://github.com/sousadevelop/Predictive_Score_Analysis/assets/92130316/a2127ae7-e684-4d02-9723-6f693209b64b)

[Modelo KNN]
![modelo_knn](https://github.com/sousadevelop/Predictive_Score_Analysis/assets/92130316/c518e248-d6ad-49e1-bafd-d14575e3d3ac)

---
### Avisos:
- Quanto maior a base de dados melhor será a análise realizada pela IA.

- Em uma empresa real deve ser usados o máximo possível de modelos de IA **dentro do contexto da empresa**.

- Quanto maior a base de dados melhor será o treinamento, porém mais irá demorar para as análises serem feitas.

- A satisfação com a porcentagem da precisão de um modelo depende do que está sendo analisado.
  - Exemplo: se for a eficâcia de um medicamento a acurácia/precisão aceita é sempre de 99%. Mas se for a precisão de uma venda de um produto +80% já está bom.
> Este projeto foi fruto da aula de Imersão em Python da Hashtag Treinamentos
