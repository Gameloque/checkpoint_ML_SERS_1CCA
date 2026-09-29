
# Checkpoint_ML_SERS_1CCA - ATIVIDADE DE REGRESSÃO LINEAR E ANALISE PREDITIVA COM 
Integrantes:

Arthur de Oliveira Cavralho - RM: 573499

Gabriel Henrique S. de Melo Rodrigues - RM: 573093

Fernando Bonfim Hoefle - RM: 569920

Anna Cecília Guimarães M. Lima de Carvalho - RM: 570955

# Machine Learning com APIs Públicas

# Objetivo

Este projeto utiliza dados obtidos por APIs públicas para desenvolver duas tarefas de Machine Learning:

* Classificação da fonte de geração de energia de empreendimentos cadastrados na ANEEL.
* 
* Regressão para estimar a radiação solar em Petrolina (PE) a partir de dados meteorológicos.

# Fontes dos Dados

ANEEL – Sistema de Informações de Geração (SIGA)

Fonte:
https://dadosabertos.aneel.gov.br/dataset/siga-sistema-de-informacoes-de-geracao-da-aneel

Foram utilizados dados de potência instalada e localização dos empreendimentos para classificar as fontes de geração em Solar, Eólica e Hidráulica.

Open-Meteo Historical Weather API

Fonte:
https://open-meteo.com/en/docs/historical-weather-api

Local analisado: Petrolina (PE)

Período: 01/04/2025 a 30/06/2025

Foram utilizados registros horários entre 7h e 17h para estimar a radiação solar.

# part4 - CP2

# Tarefa 1 – Classificação

Variáveis utilizadas:

* Potência instalada
  
* Latitude
  
* Longitude

Modelos comparados:

* Random Forest
  
* KNN
  
* Regressão Logística

Métricas utilizadas:

* Accuracy
 
* Precision
  
* Recall
  
* F1-Score
  
* Matriz de Confusão

# Tarefa 2 – Regressão

Variáveis utilizadas:

* Temperatura
  
* Umidade
  
* Cobertura de nuvens
  
* Velocidade do vento
  
* Hora

Modelos comparados:

* Regressão Linear
  
* Árvore de Decisão
  
* Random Forest

Métricas utilizadas:

* MAE
  
* MSE
  
* R²

A divisão dos dados foi feita utilizando os primeiros 80% dos registros para treino e os últimos 20% para teste.

# Como Executar

1. Clone o repositório.
   
3. Instale as dependências:

pip install pandas numpy matplotlib scikit-learn requests

3. Abra os notebooks no Jupyter Notebook ou Google Colab.

4. Execute as células na ordem apresentada.

# Conclusão

Na tarefa de classificação, os modelos conseguiram identificar padrões entre os diferentes tipos de empreendimentos utilizando potência e localização. Na tarefa de regressão, foi possível estimar a radiação solar a partir de variáveis meteorológicas, com destaque para a influência da hora do dia e da cobertura de nuvens. A comparação entre os modelos permitiu avaliar diferentes abordagens utilizando os mesmos conjuntos de dados.
