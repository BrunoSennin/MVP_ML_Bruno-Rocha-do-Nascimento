# MVP Machine Learning – Predição de Contratação de Candidatos

## 📋 Descrição do Projeto

Este projeto tem como objetivo desenvolver um modelo de Machine Learning capaz de prever a decisão de contratação de candidatos com base em informações obtidas durante um processo seletivo.

O trabalho foi desenvolvido como MVP (Minimum Viable Product) da disciplina de Machine Learning & Analytics, seguindo todas as etapas do ciclo de vida de um projeto de ciência de dados: definição do problema, análise exploratória, preparação dos dados, modelagem, otimização de hiperparâmetros, avaliação e interpretação dos resultados.

---

## 🎯 Objetivo

Construir um modelo capaz de prever a variável:

**HiringDecision**

onde:

- 0 = Não Contratar
- 1 = Contratar

O objetivo é identificar quais fatores influenciam a decisão final de contratação e avaliar a capacidade dos algoritmos de Machine Learning em apoiar esse processo.

---

## 📊 Dataset

**Base utilizada:** Predicting Hiring Decisions in Recruitment Data

**Fonte:** Kaggle

O dataset contém informações relacionadas a:

- Idade
- Gênero
- Escolaridade
- Anos de experiência
- Número de empresas anteriores
- Distância até a empresa
- Pontuação técnica (SkillScore)
- Pontuação em entrevista (InterviewScore)
- Avaliação comportamental (PersonalityScore)
- Estratégia de recrutamento (RecruitmentStrategy)

Variável alvo:

- HiringDecision

---

## 🔎 Principais Hipóteses

Durante a análise exploratória foram levantadas as seguintes hipóteses:

- Candidatos com maior SkillScore possuem maior probabilidade de contratação.
- Melhor desempenho em entrevistas aumenta a chance de contratação.
- Características comportamentais influenciam a decisão final.
- A estratégia de recrutamento utilizada impacta diretamente os resultados.

---

## 🤖 Modelos Avaliados

Foram avaliados os seguintes modelos:

- Baseline (Dummy Classifier)
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- Random Forest Otimizada (GridSearchCV)

---

## ⚙️ Otimização de Hiperparâmetros

O modelo Random Forest foi selecionado para otimização utilizando:

- GridSearchCV
- Validação Cruzada (5 folds)
- Métrica principal: F1-Score

Hiperparâmetros ajustados:

- n_estimators
- max_depth
- min_samples_split
- min_samples_leaf

---

## 📈 Resultados

### Melhor Modelo

Random Forest

### Métricas no Conjunto de Teste

| Métrica | Resultado |
|----------|----------|
| Accuracy | 0.9367 |
| Precision | 0.9405 |
| Recall | 0.8495 |
| F1-Score | 0.8927 |

---

## 🔍 Principais Descobertas

As variáveis mais importantes para a previsão da contratação foram:

1. RecruitmentStrategy
2. SkillScore
3. InterviewScore
4. PersonalityScore

Além disso, testes realizados sem a variável RecruitmentStrategy mostraram redução de desempenho, reforçando sua relevância para o modelo.

---

## ⚠️ Limitações

- Dataset sintético e educacional.
- Não houve validação em bases externas.
- Forte dependência da variável RecruitmentStrategy.
- Possíveis vieses associados a variáveis sensíveis, como Gender.

---

## 🚀 Próximos Passos

- Validar o modelo em dados reais de recrutamento.
- Expandir o conjunto de variáveis analisadas.
- Avaliar métricas de fairness algorítmica.
- Explorar modelos mais avançados de ensemble.
- Aplicar técnicas adicionais de interpretabilidade.

---

## 🛠 Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab

---

## 📌 Autor

Bruno Rocha do Nascimento

MVP – Machine Learning & Analytics
