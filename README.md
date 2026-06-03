# Iris Flower Classification using K-Nearest Neighbors (KNN)

🇧🇷 Português | 🇺🇸 English

---

# 🇧🇷 Português

## Sobre o Projeto

Este projeto aplica técnicas de Machine Learning para classificar espécies de flores do conjunto de dados Iris utilizando o algoritmo K-Nearest Neighbors (KNN).

O objetivo é prever a espécie de uma flor com base em suas características morfológicas, demonstrando conceitos fundamentais de classificação supervisionada, pré-processamento de dados e avaliação de modelos.

---

## Objetivo

Desenvolver um modelo capaz de identificar a espécie de uma flor Iris a partir de suas medidas físicas.

As espécies presentes no dataset são:

* Iris Setosa
* Iris Versicolor
* Iris Virginica

---

## Dataset

O projeto utiliza o famoso Iris Dataset, amplamente empregado no ensino e estudo de Machine Learning.

### Variáveis Utilizadas

| Variável     | Descrição             |
| ------------ | --------------------- |
| Sepal Length | Comprimento da sépala |
| Sepal Width  | Largura da sépala     |
| Petal Length | Comprimento da pétala |
| Petal Width  | Largura da pétala     |

### Variável Alvo

| Variável | Descrição       |
| -------- | --------------- |
| Species  | Espécie da flor |

---

## Análise Exploratória dos Dados

Foram realizadas etapas de exploração dos dados, incluindo:

* Visualização das primeiras linhas do dataset;
* Contagem das amostras de cada espécie;
* Análise gráfica da distribuição das flores utilizando gráficos de dispersão.

Essas análises ajudam a compreender a estrutura dos dados antes do treinamento do modelo.

---

## Pré-processamento

Como o algoritmo KNN é baseado em cálculos de distância entre observações, foi necessário realizar a normalização dos dados.

Foi utilizado o método:

* MinMaxScaler

Esse processo transforma todas as variáveis para uma escala entre 0 e 1, evitando que atributos com valores maiores tenham influência excessiva nos cálculos de distância.

---

## Modelo Utilizado

### K-Nearest Neighbors (KNN)

O KNN é um algoritmo de classificação supervisionada baseado na proximidade entre observações.

Para classificar uma nova amostra:

1. O algoritmo calcula a distância entre a nova observação e todas as amostras de treinamento;
2. Seleciona os K vizinhos mais próximos;
3. Realiza uma votação entre os vizinhos;
4. A classe mais votada é atribuída à nova observação.

Neste projeto foi utilizado:

```python
K = 5
```

---

## Divisão dos Dados

Os dados foram divididos em:

* 70% para treinamento;
* 30% para teste.

A divisão foi realizada utilizando a função `train_test_split()` do Scikit-Learn.

---

## Avaliação do Modelo

O desempenho foi avaliado utilizando:

### Accuracy

Mede a porcentagem de classificações corretas realizadas pelo modelo.

### Classification Report

Apresenta métricas como:

* Precision
* Recall
* F1-Score

para cada espécie.

### Confusion Matrix

Permite visualizar os acertos e erros de classificação para cada classe.

---

## Previsão de Novos Dados

Após o treinamento, o modelo foi utilizado para prever a espécie de uma nova flor com as seguintes características:

```python
[5.1, 3.5, 1.4, 0.2]
```

Demonstrando uma aplicação prática do modelo treinado.

---

## Conclusão

O algoritmo KNN apresentou excelente desempenho na classificação das espécies do dataset Iris.

Além de demonstrar conceitos importantes de classificação supervisionada, o projeto evidenciou a importância da normalização dos dados para algoritmos baseados em distância.

---

# 🇺🇸 English

## About the Project

This project applies Machine Learning techniques to classify Iris flower species using the K-Nearest Neighbors (KNN) algorithm.

The objective is to predict the species of a flower based on its morphological measurements while demonstrating supervised classification, data preprocessing, and model evaluation concepts.

---

## Objective

Build a model capable of identifying Iris flower species based on physical measurements.

The dataset contains three species:

* Iris Setosa
* Iris Versicolor
* Iris Virginica

---

## Dataset

The project uses the famous Iris Dataset, one of the most widely used datasets in Machine Learning education and research.

### Features

| Feature      | Description         |
| ------------ | ------------------- |
| Sepal Length | Length of the sepal |
| Sepal Width  | Width of the sepal  |
| Petal Length | Length of the petal |
| Petal Width  | Width of the petal  |

### Target Variable

| Variable | Description    |
| -------- | -------------- |
| Species  | Flower species |

---

## Exploratory Data Analysis

The project includes:

* Dataset inspection;
* Class distribution analysis;
* Scatter plot visualization of flower measurements.

These steps help understand the dataset before model training.

---

## Data Preprocessing

Since KNN is a distance-based algorithm, feature scaling is required.

The project uses:

* MinMaxScaler

This technique scales all features to a range between 0 and 1, preventing variables with larger magnitudes from dominating the distance calculations.

---

## Model

### K-Nearest Neighbors (KNN)

KNN is a supervised classification algorithm based on similarity between observations.

To classify a new sample:

1. The algorithm calculates the distance between the new observation and all training samples;
2. Selects the K nearest neighbors;
3. Performs a majority vote;
4. Assigns the most frequent class to the new observation.

The model was configured with:

```python
K = 5
```

---

## Data Split

The dataset was divided into:

* 70% training data;
* 30% testing data.

The split was performed using Scikit-Learn's `train_test_split()` function.

---

## Model Evaluation

The model was evaluated using:

### Accuracy

Measures the percentage of correct predictions.

### Classification Report

Provides:

* Precision
* Recall
* F1-Score

for each class.

### Confusion Matrix

Displays classification performance for each species.

---

## Prediction of New Samples

After training, the model was used to predict the species of a new flower with the following measurements:

```python
[5.1, 3.5, 1.4, 0.2]
```

Demonstrating a practical application of the trained classifier.

---

## Conclusion

The KNN algorithm achieved excellent performance in classifying Iris flower species.

The project also highlights the importance of feature scaling when working with distance-based Machine Learning algorithms.

---

## Technologies

* Python
* Pandas
* Scikit-Learn
* Seaborn
* Matplotlib

---

## Author

Flávia Vitória de Queiroz

