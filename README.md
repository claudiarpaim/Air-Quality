# Air Quality Prediction using Neural Networks

<p align="center">
  <img src="figure/capa.png" alt="Capa do projeto" width="700"/>
</p>

# Visão Geral do Projeto

Este projeto aplica técnicas de Ciência de Dados e Redes Neurais Artificiais para prever a concentração de Benzeno (C6H6) a partir de respostas de sensores químicos e variáveis meteorológicas. O estudo foi desenvolvido com foco em modelagem preditiva, comparação entre modelos lineares e não lineares e interpretação crítica dos resultados — seguindo boas práticas esperadas em um ambiente profissional.

O projeto utiliza o Air Quality Dataset (UCI Machine Learning Repository), amplamente conhecido na literatura, mas explorado aqui com uma abordagem estruturada, didática e orientada a negócio.

# Objetivo

Construir e avaliar modelos preditivos capazes de estimar a concentração real de Benzeno (C6H6(GT)) utilizando:

- Respostas de sensores de óxidos metálicos
- Variáveis meteorológicas
- Técnicas de Machine Learning e Redes Neurais

## Dataset

- **Fonte**: UCI Machine Learning Repository – Air Quality Dataset
- **Nome**: Air Quality Dataset
- **Link oficial**: https://archive.ics.uci.edu/ml/datasets/Air+Quality
- **Descrição**: Medições horárias de poluentes atmosféricos obtidas por sensores químicos e analisadores de referência certificados.
- **Variável alvo**: C6H6(GT) – concentração real de benzeno

⚠️ Observação: O dataset não está versionado neste repositório devido ao seu tamanho.

# Etapas do Projeto

## 1. Análise Exploratória dos Dados (EDA)

- Inspeção de variáveis
- Identificação de valores ausentes
- Análise estatística inicial

<p align="center">
  <img src="figure/distribuicao_alvo.png" alt="Capa do projeto" width="700"/>
</p>

<p align="center">
  <img src="figure/correlação_c6h6.png" alt="Capa do projeto" width="700"/>
</p>

## 2. Pré-processamento

- Tratamento de valores ausentes
- Remoção de colunas irrelevantes
- Padronização das variáveis
- Separação em conjuntos de treino e teste

## 3. Modelagem Preditiva

- Regressão Linear (baseline)

<p align="center">
  <img src="figure/regressao_model.png" alt="Capa do projeto" width="700"/>
</p>
  
- Rede Neural do tipo MLP (Multilayer Perceptron)

<p align="center">
  <img src="figure/mlp_model.png" alt="Capa do projeto" width="700"/>
</p>

## 4. Avaliação dos Modelos

- RMSE
- MAE
- R²
- Comparação de Desempenho dos Modelos

| Modelo             | RMSE     | MAE      | R²       |
|--------------------|----------|----------|----------|
| Regressão Linear   | 1.181182 | 0.836396 | 0.974607 |
| Rede Neural (MLP)  | 0.093018 | 0.057397 | 0.999843 |
  

# Modelos Utilizados

##🔹 Regressão Linear (Baseline)
Modelo utilizado como referência para avaliar ganhos obtidos com modelos não lineares.

##🔹 Rede Neural Artificial (MLP)

- Arquitetura feedforward
- Funções de ativação não lineares
- Capaz de capturar relações complexas entre sensores e concentração de poluentes

# Principais Resultados

A Rede Neural apresentou desempenho superior ao modelo linear, indicando que:
- A relação entre sensores e concentração de benzeno não é puramente linear
- Modelos baseados em ANN são mais adequados para esse tipo de problema ambiental
