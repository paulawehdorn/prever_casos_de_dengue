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

### 3.3. Atributos que influenciam a previsão:
- O dicionário de dados encontra-se no [item 8](#8-dicionário-de-dados).

### 3.4. Métrica de desempenho:

A métrica de desempenho escolhida é o [Root Mean Squared Error (RMSE)](https://docs.oracle.com/cloud/help/pt_BR/pbcs_common/PFUSU/insights_metrics_RMSE.htm#PFUSU-GUID-FD9381A1-81E1-4F6D-8EC4-82A6CE2A6E74), que é adequada para medir a precisão de previsões contínuas, penalizando grandes desvios.

## 4. Conclusões

## 5. Próximos passos

Um relatório de explanação contendo:
- Análise descritiva: Examinando os dados históricos.
- Análise preditiva: Previsões futuras baseadas em modelos de ML.
- Análise diagnóstica: Identificação de fatores que contribuem para os casos de dengue.
- Análise prescritiva: Recomendações de ações baseadas nas previsões.

## 6. Tecnologias Utilizadas

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

## 8. Dicionário de dados

FEATURE	| DESCRIPTION
-- | --
Date | Data das informações
Casos de dengue | Total de número de casos observados no dia
Presença de mosquito | Quantidade de mosquitos observada
Precipitação | Água proveniente do vapor de água atmosférica depositada na superfície
Umidade | Relação entre a pressão parcial da água contida no ar e a pressão de vapor da água à temperatura do ar
Temperatura | Calor da atmosfera, em graus Celsius (ºC)
Conscientização da População | Nível de conscientização sobre a dengue
Condições de Moradia Precárias | Taxa de moradias precárias na área observada
Falta de Acesso a Serviços de Saúde | Taxa de moradores sem acesso a serviços de saúde
Migração de Pessoas de Áreas Endêmicas | Taxa de migração entre áreas
Transporte de Mercadorias em Áreas Urbanas | % de veículos de transporte de cargas
Presença de Criadouros | % da área com presença de mosquitos
Água Parada em Terrenos Baldios | % da área com presença de água parada
Presença de Piscinas sem Manutenção | Número de piscinas sem manutenção observadas
Presença de Recipientes sem Tampas | Número de recipientes observados no dia
Falta de Coleta de Lixo | Taxa de coleta de lixo realizada
Área com Acúmulo de Entulho | % da área com entulho
Falta de Controle de Pragas | % da área observada sem controle de pragas
Taxa de Tratamento de Esgoto | % de esgoto não tratado na área observada
Status | Status de conscientização da população
Id | Identificador único do registro

## 9. Estrutura de Pastas
```plaintext
├── data
│   ├── tb_fato.csv
│   ├── tb_casos_dengue.csv
│   ├── tb_agua_parada.csv
│   ├── tb_condicoes_climaticas.csv
│   ├── tb_falta_higiene.csv
│   └── tb_conscientizacao.csv
├── img
├── models
│   └── model.pkl
├── notebooks
│   └── prever_casos_de_dengue.ipynb
├── README.md
└── requirements.txt