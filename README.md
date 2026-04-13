# PUC_MVP_Analise_de_Dados

Este repositório contém o MVP (Minimum Viable Product) desenvolvido para a pós-graduação em Análise e Ciência de Dados da **PUC-Rio**.  
O projeto consiste em uma análise exploratória de dados (EDA), teste de hipóteses e engenharia de variáveis aplicada a séries temporais do preço do ouro, com o objetivo de identificar padrões estatísticos e comportamentais relevantes.

## Definição do Problema
O objetivo deste trabalho é analisar o dataset **Gold Price (2005–2026) Historical Price Data**, com foco em compreender o comportamento do preço do ouro ao longo do tempo. A análise busca identificar padrões estatísticos, regimes de volatilidade e relações entre variáveis de mercado, além de avaliar a capacidade preditiva de variáveis derivadas (como retornos e médias móveis) na previsão da direção futura do preço (alta ou queda). 

## Estrutura do Projeto
O notebook está organizado seguindo o ciclo de vida de um projeto de ciência de dados:

1. **Carga e Descrição dos Dados:** Importação do dataset e entendimento inicial das variáveis.
2. **Tratamento de Dados:** Limpeza, tratamento de valores ausentes e construção de variáveis derivadas.
3. **Análise Exploratória (EDA):** Estatísticas descritivas, distribuições, correlações e visualizações.
4. **Análise de Hipóteses:** Validação empírica de suposições sobre o comportamento do ativo.
5. **Modelagem Preditiva:** Construção de modelo supervisionado para previsão da direção do preço.
6. **Conclusões e Insights:** Síntese dos resultados e limitações do modelo.

## Principais Insights
### **Hipótese 1: Correlação entre variáveis de preço (Confirmada)**
Foi identificada forte correlação entre preço de abertura, fechamento, máxima e mínima, o que indica alta redundância informacional entre essas variáveis. Isso sugere que, para modelagem preditiva, é possível reduzir dimensionalidade sem perda significativa de informação.
### **Hipótese 2: Distribuição dos retornos diários (Confirmada)**
Os retornos apresentam distribuição centrada em torno de zero, com presença de caudas pesadas e valores extremos. Esse comportamento é característico de séries financeiras e reflete a ocorrência de choques de mercado e alta volatilidade.
### **Hipótese 3: Poder preditivo de variáveis derivadas (Parcialmente confirmada)**
Variáveis como médias móveis, retornos defasados e volatilidade capturam padrões relevantes de tendência. No entanto, o desempenho do modelo preditivo foi próximo ao baseline, sugerindo que fatores externos ao dataset influenciam fortemente a direção do preço do ouro.
### **Hipótese 4: Influência de regimes macroeconômicos (Confirmada)**
O comportamento do ouro varia significativamente em diferentes regimes macroeconômicos. Em períodos de crise (2008 e COVID-19), observa-se aumento expressivo da volatilidade e alterações na distribuição dos retornos, evidenciando o papel do ouro como ativo de proteção em momentos de estresse financeiro.
### **Hipótese 5: Dependência do horizonte temporal (Confirmada)**
A análise de janelas temporais (12, 24 e 36 meses) indica que o curto prazo é mais ruidoso e menos previsível, enquanto horizontes mais longos tendem a suavizar a volatilidade e revelar tendências estruturais mais estáveis.

## Tecnologias Utilizadas
* **Linguagem:** Python 3.x  
* **Bibliotecas:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
* **Ambiente:** Google Colab / Jupyter Notebook 

## Como visualizar o projeto
Você pode acessar o notebook diretamente pelos links abaixo:

* [Visualizar no GitHub](https://github.com/lalipedrozo/PUC_MVP_Analise_de_Dados/blob/main/PUC_MVP_Analise_de_Dados.ipynb)
* [Abrir no Google Colab](https://colab.research.google.com/github/lalipedrozo/PUC_MVP_Analise_de_Dados/blob/main/PUC_MVP_Analise_de_Dados.ipynb)

## Observação
Este projeto tem caráter exploratório e educacional, focado na aplicação de técnicas de análise de dados e modelagem preditiva em séries temporais financeiras.

**Autor:** Larissa de Almeida Leite Pedrozo  
**Instituição:** PUC-Rio - Pós-graduação em Análise e Ciência de Dados
**Contexto:** MVP de Pós-Graduação em Data Science & Analytics - PUC-Rio
