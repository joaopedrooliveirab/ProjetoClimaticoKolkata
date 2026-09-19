#  Projeto Climático Kolkata

Pipeline de dados meteorológicos desenvolvido para praticar conceitos de Engenharia de Dados utilizando arquitetura Medalhão (Bronze, Silver e Gold), Python, Pandas, SQLite e Streamlit.

##  Objetivo

O projeto tem como objetivo construir um pipeline de dados capaz de:

- realizar a ingestão de dados meteorológicos;
- armazenar os dados na camada Bronze;
- realizar limpeza, padronização e validação na camada Silver;
- gerar métricas e agregações na camada Gold;
- disponibilizar os resultados por meio de um dashboard interativo em Streamlit.

##  Arquitetura

O projeto utiliza uma arquitetura Medalhão composta por três camadas:

###  Bronze
Armazena os dados brutos, preservando as informações conforme foram recebidas da fonte.

###  Silver
Realiza o tratamento e a padronização dos dados, incluindo limpeza, conversão de tipos, validações e demais transformações necessárias.

###  Gold
Armazena os dados preparados para análise, incluindo métricas, agregações e informações utilizadas pelo dashboard.

### Fluxo

CSV → Bronze → Silver → Gold → Streamlit

O SQLite é utilizado como mecanismo de armazenamento das diferentes camadas do pipeline.

##  Tecnologias

- Python
- Pandas
- SQLite
- Streamlit
- Git / GitHub

##  Dataset

Os dados utilizados neste projeto foram obtidos a partir do Kaggle.

**Dataset:** [Kolkata Climate and Weather (2021–2025) Daily Data](https://www.kaggle.com/datasets/sumanbera19/kolkata-climate-and-weather-20212025-daily-data)

**Autor atribuído no Kaggle:** Suman Bera

**Licença do dataset:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

Os dados foram utilizados como fonte para o pipeline de Engenharia de Dados desenvolvido neste projeto.

##  Pipeline

```text
Dataset CSV
    ↓
Ingestão
    ↓
 Bronze
Dados brutos
    ↓
 Silver
Limpeza + Padronização + Validação
    ↓
 Gold
Métricas + Agregações
    ↓
Streamlit
Dashboard e visualização

## O projeto pretende investigar questões como:
Qual mês apresentou maior precipitação?
Qual ano apresentou a maior temperatura média?
Quais condições climáticas ocorreram com maior frequência?
Quais foram os dias mais quentes e mais frios?
Como a precipitação varia ao longo dos meses?
Em quais períodos os ventos foram mais fortes?

## Objetivo de aprendizado

### Este projeto está sendo desenvolvido com foco em aprendizado prático dos conceitos de:

ingestão de dados
armazenamento
arquitetura Medalhão
tratamento e qualidade de dados
transformação de dados
agregação e criação de métricas
visualização de dados
versionamento com Git e GitHub.