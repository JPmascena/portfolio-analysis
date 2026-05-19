# Análise Quantitativa e Previsão do Mercado Financeiro com Machine Learning

## Visão Geral

Este projeto aplica técnicas de Ciência de Dados, Finanças Quantitativas e Machine Learning para análise de ativos financeiros, gerenciamento de risco e previsão de movimentos do mercado.

O estudo utiliza dados históricos do mercado brasileiro e internacional para avaliar:
- risco
- retorno
- volatilidade
- diversificação
- previsão de ativos
- performance de portfólio

Além disso, o período da pandemia foi removido da análise devido à quebra estrutural causada pela extrema volatilidade do mercado.

---

# Objetivo

O objetivo principal do projeto é investigar como variáveis macroeconômicas e financeiras podem auxiliar na previsão do comportamento do mercado financeiro e na construção de estratégias quantitativas.

O projeto também busca:
- avaliar risco e retorno
- analisar diversificação
- aplicar métricas quantitativas
- testar modelos de Machine Learning
- realizar backtesting de estratégias

---

# Ativos Utilizados

| Ativo | Ticker |
|---|---|
| IBOVESPA | ^BVSP |
| S&P500 | ^GSPC |
| VIX | ^VIX |
| Dólar | USDBRL=X |
| Ouro | GC=F |
| IPCA | Banco Central do Brasil |

---

# Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- yfinance
- Jupyter Notebook

---

# Metodologia

## 1. Coleta de Dados

Os dados históricos foram coletados utilizando:
- Yahoo Finance API
- API do Banco Central do Brasil

O período analisado compreende dados entre 2014 e 2025.

---

## 2. Tratamento dos Dados

Foram realizados:
- limpeza de dados
- tratamento de valores nulos
- alinhamento temporal
- padronização das séries históricas

## 3. Remoção da Pandemia

O período da pandemia foi removido do treinamento do modelo devido à quebra estrutural causada pela COVID-19 nos mercados financeiros.

Essa abordagem reduz distorções estatísticas e melhora a estabilidade da modelagem.

## 4. Engenharia de Features

Foram criadas variáveis derivadas como:
- retornos logarítmicos
- volatilidade móvel
- médias móveis
- momentum
- correlação dinâmica

## 5. Modelagem

Foi utilizado o modelo Random Forest para identificação de padrões históricos e previsão do comportamento do mercado.

# Métricas Financeiras

O projeto utiliza métricas quantitativas como:

- Value at Risk (VaR)
- Conditional Value at Risk (CVaR)
- Volatilidade
- Correlação
- Drawdown
- Sharpe Ratio
- Retorno acumulado

# Resultados

Os resultados demonstraram que:

- portfólios diversificados reduziram o risco total
- o VIX apresentou maior volatilidade
- o S&P500 apresentou crescimento mais consistente
- o ouro funcionou como ativo de proteção
- o modelo conseguiu identificar padrões relevantes entre variáveis macroeconômicas e movimentos do mercado

---

# Estrutura do Projeto

portfolio-analysis/
│
├── data/
├── notebooks/
├── src/
├── images/
├── reports/
├── models/
├── README.md
└── requirements.txt

---

# Como Executar

```bash
git clone https://github.com/JPmascena/Portfolio-Analysis.git

cd Portfolio-Analysis

pip install -r requirements.txt

jupyter notebook
