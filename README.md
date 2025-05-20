# 🌳 Relatório de Experimentos com Árvores de Decisão

## 👩‍💻 Autores
- Rafaela P. M. Fernandes  
- Atharv Nuthi  
Instituto de Computação – Universidade Federal Fluminense (UFF)  
Emails: rafaelapecanha@id.uff.br, atharvnuthi@id.uff.br  

## 📘 Descrição

Este repositório apresenta experimentos utilizando algoritmos baseados em **árvores de decisão** aplicados a dois conjuntos de dados clássicos: **Iris** e **Breast Cancer Wisconsin (Diagnostic)**. O objetivo foi avaliar o desempenho de modelos supervisionados utilizando as abordagens **CART** e **Random Forest**, explorando também aspectos como **poda**, **validação cruzada**, **outliers** e **ajuste de threshold**.

## 🧪 Experimentos Realizados

### 🌺 Dataset Iris
- Classificação das espécies *Setosa*, *Versicolor* e *Virginica*.
- Utilizado o algoritmo **CART** com critério de impureza Gini.
- Avaliação com **validação cruzada 10-fold**.

### 🧬 Dataset Breast Cancer Wisconsin
- Classificação de tumores como **benignos** ou **malignos**.
- Utilização de **Random Forest** com ajustes no **threshold de decisão**.
- Análise comparativa entre modelos **com e sem outliers** (identificados via IQR).
- Avaliação com **relatório de classificação** e **matriz de confusão**.
- Poda não aplicada na Random Forest (não é usual neste algoritmo).

## ⚙️ Tecnologias e Bibliotecas

- Python 3.10+
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn

## 📊 Principais Resultados

- **Modelo com outliers** obteve acurácia de **96%**, superando o modelo sem outliers (93%).
- A presença de outliers contribuiu positivamente na identificação da classe **maligna**, contendo informações relevantes.
- A matriz de confusão revelou **alta sensibilidade e precisão** no modelo com outliers (ex: 103 VP, 62 VN).

## 📁 Estrutura do Repositório

├── breast_cancer.ipynb # Notebook com experimento no dataset Breast Cancer
├── iris_classification.ipynb # Notebook com experimento no dataset Iris
├── data/ # Conjuntos de dados (se necessário)
├── README.md # Este arquivo