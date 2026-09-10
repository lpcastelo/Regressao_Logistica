# Regressão Logísticaaaa
Aqui você irá encontrar a atividade do módulo 27 do curso de Cientista de Dados da Ebac.

A atividade consiste em desenvolver um modelo de Regressão Logística para classificar se uma pessoa possui ou não doenças cardíacas, utilizando técnicas de análise de dados e avaliação de modelos de Machine Learning.

Durante a atividade serão abordados temas como:

* Análise exploratória de dados (EDA)
* Regressão Logística
* Classificação supervisionada
* Métricas de desempenho como precisão, recall e f1-score
* Curva ROC e métrica AUC

O objetivo é compreender como a Regressão Logística pode ser aplicada em problemas de classificação, além de interpretar métricas importantes para avaliar a qualidade e a capacidade preditiva do modelo.

## Dados

Base `CARDIO_BASE.csv` (10.000 pacientes), com variáveis como idade, altura, peso, colesterol, glicose, tabagismo, consumo de álcool e atividade física, e a variável alvo `cardio_disease`. Foram tratados um erro de formatação na coluna `weight` (vírgula como separador decimal) e um outlier de altura (250 cm).

## Resultados

O modelo (dados padronizados, já balanceados) alcançou **64% de acurácia** tanto no treino quanto no teste, com AUC de 0,64 — um desempenho considerado fraco (a meta discutida no notebook era acima de 0,80). As variáveis com maior correlação com a doença cardíaca foram idade, peso e colesterol, mas isso não foi suficiente para um modelo linear simples separar bem as classes.

## Tecnologias

- Python, pandas
- scikit-learn (LogisticRegression, StandardScaler, métricas)
- imbalanced-learn (SMOTE, importado mas não necessário — base já balanceada)
- matplotlib, seaborn

## Como executar

1. Instale as dependências: `pip install pandas scikit-learn imbalanced-learn matplotlib seaborn`.
2. Coloque `CARDIO_BASE.csv` no mesmo diretório do notebook.
3. Execute `Profissao Cientista de Dados M27 Pratique.ipynb` em ordem.
