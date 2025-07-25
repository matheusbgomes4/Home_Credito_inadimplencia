# 🏦 Home Credit Default Risk - Previsão de Inadimplência com Machine Learning

Este projeto tem como objetivo prever o risco de inadimplência de clientes utilizando os dados da competição [Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk) da plataforma Kaggle. A proposta é aplicar técnicas de Ciência de Dados e algoritmos de Machine Learning para identificar padrões de comportamento e construir um modelo preditivo eficaz.

---

## 📘 Resumo do Projeto

A inadimplência é um dos principais desafios enfrentados por instituições financeiras. Com base em um conjunto robusto de dados financeiros, históricos de crédito e registros de comportamento dos clientes, este projeto constrói um pipeline completo que envolve:

- Integração de múltiplas bases de dados (`application_train`, `bureau`, `previous_application`, `credit_card_balance`, etc.)
- Engenharia de atributos com agregações por cliente (`groupby().agg()`)
- Pré-processamento e tratamento de dados ausentes
- Treinamento de um modelo preditivo utilizando **LightGBM**
- Avaliação da performance com a métrica AUC

---

## 🧠 Técnicas Utilizadas

- Análise exploratória de dados (EDA)
- Engenharia de atributos com agregações
- Tratamento de valores ausentes
- Modelagem preditiva com **LightGBM**
- Avaliação de performance com **AUC**
- Interpretação com gráfico de importância das features

---

## 📂 Estrutura do Projeto
# 📁 home-credit-default-risk/
- Kagle_Home_Credit.ipynb # Notebook principal do projeto
- application_train.csv # Base principal (não incluída no repositório)
- bureau.csv # Histórico de crédito externo
- previous_application.csv # Aplicações anteriores
- credit_card_balance.csv # Saldos de cartão de crédito
- README.md # Este arquivo
---

## 📊 Resultados Obtidos

- **Modelo utilizado:** LightGBM (sem ensemble)
- **Métrica de avaliação:** AUC (Área sob a Curva ROC)
- **Score (validação local):** AUC ≈ 0.74
