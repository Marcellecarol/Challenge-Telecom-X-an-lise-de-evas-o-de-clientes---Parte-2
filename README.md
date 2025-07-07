# Challenge-Telecom-X-an-lise-de-evas-o-de-clientes---Parte-2
Previsão de Churn em TelecomX 📋 Descrição Este projeto realiza uma análise e modelagem preditiva para identificar clientes que provavelmente irão cancelar (churn) o serviço da empresa de telecomunicações fictícia TelecomX. Utilizando dados JSON com informações demográficas, de serviço e conta, o objetivo é construir modelos que ajudem a prever o churn com boa acurácia.

🗂️ Dados Os dados foram obtidos de uma fonte pública no formato JSON, contendo informações aninhadas sobre clientes, telefone, internet e conta:

customer: dados demográficos do cliente (gênero, dependentes, tempo como cliente, etc.)

phone: serviços telefônicos contratados

internet: serviços de internet contratados

account: informações de pagamento e contratos

churn: variável alvo indicando se o cliente cancelou ou não

⚙️ Tecnologias e Bibliotecas Python 3.x

pandas

numpy

seaborn

matplotlib

scikit-learn

🚀 Passos do projeto Carregamento e preparação dos dados

Leitura dos dados JSON da URL

Expansão das colunas aninhadas com pd.json_normalize

Combinação dos dados em um DataFrame único

Padronização dos nomes das colunas e tipos de dados

Tratamento de valores faltantes e normalização textual

Engenharia de dados

Codificação da variável alvo (churn) para valores binários

One-hot encoding para variáveis categóricas

Escalonamento dos dados numéricos

Modelagem

Separação dos dados em treino e teste (30% teste)

Treinamento de três modelos:

Regressão Logística

Árvore de Decisão

Random Forest

Avaliação

Análise de métricas: matriz de confusão, relatório de classificação e ROC AUC

Visualização das 10 variáveis mais importantes no modelo Random Forest

📊 Resultados O modelo Random Forest apresentou o melhor desempenho para prever churn. As variáveis mais importantes foram exibidas em gráfico e listadas no final do código.
