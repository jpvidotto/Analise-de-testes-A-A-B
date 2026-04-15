# Análise de Testes A/B: Otimização de Funil e Conversão

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-ADADAD?style=for-the-badge)

## 📌 Visão Geral do Projeto
Este projeto analisa os resultados de um experimento de interface num aplicativo de comércio de produtos alimentares. O objetivo principal foi investigar o comportamento dos utilizadores através de um funil de vendas e validar se a alteração nas fontes do aplicativo impactaria positivamente a conversão, utilizando testes de hipóteses estatísticas.

## 🎯 Objetivos de Negócio
* **Análise do Funil:** Identificar em qual etapa os utilizadores mais abandonam o aplicativo.
* **Validação de Experimento (Teste A/B/A):** Comparar dois grupos de controlo (mesma interface) com um grupo de teste (nova fonte) para garantir a integridade dos dados e a viabilidade da mudança.
* **Tomada de Decisão Baseada em Dados:** Recomendar a implementação ou o descarte da nova interface com base na significância estatística.

## 🛠️ Stack Técnica
* **Linguagem:** Python
* **Manipulação de Dados:** Pandas, NumPy
* **Visualização:** Matplotlib, Seaborn, Plotly (Gráficos interativos de funil)
* **Estatística:** Scipy (Z-test), Statsmodels

## 📉 Metodologia e Processamento
1.  **Preparação de Dados:** Limpeza, tratamento de tipos, renomeação de colunas e filtragem de registos para garantir que o período analisado fosse íntegro (dados completos de 01/08/2019 a 07/08/2019).
2.  **Análise Exploratória (EDA):** Verificação de eventos por utilizador e distribuição por grupo experimental.
3.  **Análise de Funil:**
    * Mapeamento da jornada: `MainScreenAppear` → `OffersScreenAppear` → `CartScreenAppear` → `PaymentScreenSuccessful`.
    * Identificação de estrangulamento: Verificou-se que a maior perda de utilizadores ocorre logo após a ecrã principal.
4.  **Testes Estatísticos:**
    * Realização de testes Z para proporções entre os grupos 246, 247 (controlo) e 248 (teste).
    * Aplicação do nível de significância (Alpha) de **0.1** (ajustado para o contexto de mercado).

## 🏆 Resultados e Conclusões
* **Integridade do Teste:** Os grupos de controlo (A/A) mostraram-se estatisticamente iguais, validando o mecanismo de divisão de tráfego.
* **Desempenho da Nova Interface:** Em todos os eventos testados (Tutorial, Carrinho, Pagamento), o **P-Value foi superior ao Alpha**, indicando que não houve diferença estatisticamente significante na conversão com a nova fonte.
* **Recomendação Final:** Com base nos dados, a recomendação foi **manter a versão atual do aplicativo** e interromper o teste, economizando recursos de desenvolvimento que seriam gastos numa mudança sem impacto comprovado na faturação.

---

### 📂 Estrutura do Repositório
* `projeto11.ipynb`: Notebook Jupyter contendo toda a análise, códigos e visualizações.
* `dataframe/`: Pasta contendo os registos brutos (`logs_exp_us.csv`).

---
**João Pedro Vidotto Tavares Dias** *Data Analyst | Especialista em Vendas* [LinkedIn](https://www.linkedin.com/in/joao-vidotto/) | [GitHub](https://github.com/jpvidotto)
