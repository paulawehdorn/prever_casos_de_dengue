# Previsão de Casos de dengue

## 1. Introdução
Este é um projeto end-to-end de ciência de dados com o objetivo de prever a quantidade de casos de dengue para os próximos 1500 dias. Vamos utilizar técnicas de análise de dados e machine learning para nos possibilitar uma resposta mais proativa e eficiente no combate à doença, ajudando a salvar vidas e recursos.

## 2. Sobre o projeto
A dengue é uma doença viral transmitida principalmente pelo mosquito Aedes aegypti e representa um desafio significativo para a saúde pública devido à sua rápida disseminação e impacto na população.

### 2.1. Por que este projeto é importante?

Prever a propagação da doença permite que as autoridades de saúde implementem medidas preventivas e de controle de maneira mais eficaz, alocando recursos e intervenções precisamente nas áreas mais vulneráveis.

### 2.2. O que vamos entregar?

Uma página web com as seguintes funcionalidades:

- Previsão pontual dos casos de dengue (para um cenário específico);
- Previsão em massa dos casos de dengue (para diversos cenários).

## 3. Como vamos trabalhar?

### 3.1. Gerenciamento e organização do projeto:
- Gerenciamento: Utilizaremos o framework [SCRUM](https://www.scrum.org/resources/what-scrum-module) para gerenciamento ágil do projeto.;
- Organização: Adotaremos o framework [DM-CRISP](https://www.datascience-pm.com/crisp-dm-2/) para estruturação das etapas de ciência de dados.

### 3.2. Fontes de dados:
- Os dados utilizados neste projeto são provenientes de uma competição do  [kaggle](https://www.kaggle.com/competitions/8-hackday-comunidadeds/overview) e estão disponibilizados na pasta "data" do repositório:
  - 'tb_fato.csv';
  - 'tb_casos_dengue.csv';
  - 'tb_agua_parada.csv';
  - 'tb_condicoes_climaticas.csv';
  - 'tb_falta_higiene.csv';
  - 'tb_conscientizacao.csv'.

### **3.3. Quais as características que influenciam o número dos casos de dengue?**
- O dicionário de dados encontra-se no notebook.

### 3.4. Como será medido o desempenho do modelo de ml?

A métrica de desempenho escolhida é o [Root Mean Squared Error (RMSE)](https://docs.oracle.com/cloud/help/pt_BR/pbcs_common/PFUSU/insights_metrics_RMSE.htm#PFUSU-GUID-FD9381A1-81E1-4F6D-8EC4-82A6CE2A6E74), que é adequada para medir a precisão de previsões contínuas, penalizando grandes desvios.

## 4. Conclusões

## 5. Próximos passos

Um relatório de explanação contendo:
- Análise descritiva: Examinando os dados históricos.
- Análise preditiva: Previsões futuras baseadas em modelos de ML.
- Análise diagnóstica: Identificação de fatores que contribuem para os casos de dengue.
- Análise prescritiva: Recomendações de ações baseadas nas previsões.

## 6. Tecnologias Utilizadas

- Lista de versionamento entrontra-se no arquivo requirements.txt;
- Python;
- Pandas, Numpy, Matplotlib, Seaborn, Scikit-Learn;
- Pickle;
- Streamlit;
- Visual Studio Code;
- Git e Github.

## 7. Requisitos de Sistema
Para recriar o ambiente virtual Python, execute os seguintes comandos:

```bash
conda create -n casos_dengue python=3.12.4
conda activate casos_dengue
pip install -r requirements.txt
```