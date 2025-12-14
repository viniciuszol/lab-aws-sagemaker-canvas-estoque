# Previsão de Estoque Inteligente na AWS com SageMaker Canvas

## Visão Geral

Este projeto foi desenvolvido como parte do Lab da DIO "Previsão de Estoque Inteligente na AWS com SageMaker Canvas". O objetivo foi criar um modelo de Machine Learning utilizando o Amazon SageMaker Canvas para realizar previsões relacionadas ao contexto de estoque e precificação, utilizando dados históricos de produtos, promoções e quantidade em estoque, sem a necessidade de programação.

O SageMaker Canvas foi utilizado em todas as etapas do processo, desde a importação do dataset até a geração das previsões, explorando uma abordagem no-code para Machine Learning.

---

## Objetivo do Projeto

- Utilizar o Amazon SageMaker Canvas para criar um modelo de Machine Learning
- Aplicar conceitos de ML no-code em um cenário prático
- Analisar métricas de desempenho do modelo
- Gerar previsões a partir de novos dados
- Documentar todo o processo em um repositório GitHub

---

## Ferramentas Utilizadas

- Amazon SageMaker Canvas
- AWS Console
- Dataset em formato CSV
- GitHub para versionamento e documentação

---

## Dataset Utilizado

O modelo foi treinado com o dataset:

dataset-1000-com-preco-promocional-e-renovacao-estoque.csv

O dataset contém 1.000 registros e apresenta a seguinte estrutura:

- ID_PRODUTO (numérico): Identificador do produto
- DATA_EVENTO (datetime): Data do evento de venda
- FLAG_PROMOCAO (binário): Indica se o produto estava em promoção
- QUANTIDADE_ESTOQUE (numérico): Quantidade disponível em estoque
- PRECO (numérico): Variável alvo utilizada para treinamento do modelo

O dataset não apresentou valores ausentes ou inconsistências, permitindo um treinamento direto no SageMaker Canvas.

---

## Etapas de Desenvolvimento

### 1. Importação e Configuração dos Dados

- O dataset foi importado diretamente no Amazon SageMaker Canvas
- Os tipos de dados foram detectados automaticamente
- A coluna PRECO foi definida como variável alvo (Target)
- O Canvas recomendou automaticamente o tipo de modelo: Numeric prediction

---

### 2. Construção e Treinamento do Modelo

- Foi utilizado o modo Quick Build
- O SageMaker Canvas executou automaticamente:
  - Preparação dos dados
  - Seleção do algoritmo
  - Treinamento do modelo

O processo foi concluído rapidamente, sendo adequado para o contexto do laboratório.

---

## Avaliação do Modelo

Após o treinamento, o modelo apresentou as seguintes métricas:

- RMSE: 0.488
- MSE: 0.239

Esses valores indicam que o modelo consegue prever o preço dos produtos com um erro médio aproximado de ±0.49, o que representa um bom desempenho considerando a variação dos preços no dataset.

---

## Análise de Impacto das Variáveis

O SageMaker Canvas identificou o impacto das variáveis na previsão do preço da seguinte forma:

- ID_PRODUTO: 93.72%
- FLAG_PROMOCAO: 6.03%
- DATA_EVENTO: 0.15%
- QUANTIDADE_ESTOQUE: 0.09%

A análise mostra que o identificador do produto é o fator mais relevante para a definição do preço, seguido pela presença de promoções. As demais variáveis tiveram impacto menor neste cenário.

---

## Geração de Previsões

Foi utilizada a funcionalidade de Single Prediction para realizar previsões em tempo real.

Exemplo de dados utilizados para previsão:

- ID_PRODUTO: 100
- DATA_EVENTO: 14/11/2023
- FLAG_PROMOCAO: 0
- QUANTIDADE_ESTOQUE: 8000

Resultado da previsão:

- PRECO previsto: 153.806

Esse teste demonstra a capacidade do modelo de gerar previsões com base em novos cenários, podendo ser utilizado como apoio à tomada de decisão.

---

## Conclusão

O Amazon SageMaker Canvas demonstrou ser uma ferramenta eficiente para criação de modelos de Machine Learning no-code. O projeto permitiu aplicar conceitos práticos de ML, gerar previsões consistentes e obter insights relevantes a partir dos dados, sem a necessidade de implementação manual de algoritmos.

Esse laboratório reforça o potencial do uso de Machine Learning acessível para análise de dados e suporte a decisões estratégicas em cenários de negócio.

---

## Boas Práticas de Custo

- Realizar logout do SageMaker Canvas após o uso
- Verificar se a aplicação não permanece com status Ready
- Monitorar custos utilizando AWS Budgets
- Utilizar corretamente o Free Tier da AWS

---

## Repositório Base do Desafio

https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque

---

## Status do Projeto

Projeto concluído e pronto para entrega na plataforma da DIO.
