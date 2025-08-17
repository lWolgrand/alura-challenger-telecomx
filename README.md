# Análise de Evasão de Clientes (Churn) - Desafio Data Science

## 📝 Visão Geral do Projeto

Este projeto realiza uma análise completa sobre a evasão de clientes (churn) em uma empresa de telecomunicações fictícia, a **TelecomX**. O objetivo é seguir um processo de **ETL (Extração, Transformação e Carga)** para limpar e preparar os dados, realizar uma análise exploratória para identificar os principais fatores que influenciam o cancelamento de serviços e, por fim, gerar insights que possam orientar a tomada de decisões estratégicas para a redução do churn.

O trabalho foi desenvolvido como parte do **Challenge Data Science da Alura**.

## 📂 Estrutura do Projeto

Todo o processo foi desenvolvido em um único fluxo de trabalho, simulando um pipeline de dados. As principais etapas foram:

1.  **Extração (Extract):** Carregamento dos dados brutos a partir de um arquivo JSON.
2.  **Transformação (Transform):** Fase mais extensa, que incluiu:
    * **Limpeza de Dados:** Tratamento de valores inconsistentes e remoção de registros incompletos.
    * **Engenharia de Features:** Criação de novas colunas, como `Taxa_Diaria` e `Numero_Servicos_Adicionais`.
    * **Padronização:** Conversão de dados categóricos (ex: "Sim"/"Não") para formato numérico (1/0) e tradução das colunas para português.
3.  **Carga e Análise (Load & Analyze):** O dataset final e limpo foi utilizado para gerar análises descritivas, visualizações gráficas e uma matriz de correlação para identificar padrões.

## 🚀 Principais Descobertas e Insights

A análise revelou um perfil claro do cliente com maior propensão a cancelar o serviço. Os fatores de maior impacto são:

* **Tipo de Contrato:** Clientes com **contratos mensais** têm uma taxa de churn drasticamente maior.
* **Tempo de Contrato:** A evasão é muito mais comum entre **clientes novos** (baixo tempo de contrato).
* **Taxa Mensal:** **Cobranças mensais mais altas** estão associadas a uma maior probabilidade de churn.
* **Serviços Contratados:** Clientes com **poucos serviços adicionais** tendem a cancelar mais.

Em resumo, a falta de um compromisso de longo prazo e a sensibilidade ao preço são os principais impulsionadores da evasão de clientes.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Bibliotecas de Análise:** Pandas, NumPy
* **Bibliotecas de Visualização:** Matplotlib, Seaborn
* **Ambiente:** Google Colab / Jupyter Notebook

## ▶️ Como Executar o Projeto

Todo o pipeline de ETL e análise está contido no notebook principal (`.ipynb`). Para reproduzir os resultados, basta executar as células do notebook em sequência.

1.  Clone o repositório:
    ```bash
    git clone [https://github.com/lWolgrand/alura-challenger-telecomx.git]
    ```
2.  Abra o notebook no ambiente de sua preferência (Google Colab, Jupyter, etc.).
3.  Execute todas as células. O script foi construído para buscar os dados remotamente e gerar todas as análises e gráficos automaticamente.

---