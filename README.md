# Air Quality Prediction using Neural Networks
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

## 2. Pré-processamento

- Tratamento de valores ausentes
- Remoção de colunas irrelevantes
- Padronização das variáveis
- Separação em conjuntos de treino e teste

## 3. Modelagem Preditiva

- Regressão Linear (baseline)
- Rede Neural do tipo MLP (Multilayer Perceptron)

## 4. Avaliação dos Modelos

- RMSE
- MAE
- R²
- Comparação entre modelos

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
