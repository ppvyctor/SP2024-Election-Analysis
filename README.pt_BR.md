<br>

\[**[🇧🇷Português](README.pt_BR.md)**\] \[[🇺🇸English](README.md)\]

  <!--  START HEADER  -->

<!--  INÍCIO DO CABEÇALHO  -->
## <p align="center"> 📊 Análise de Dados e Visualização: Eleições Municipais de São Paulo - 1º e 2º Turno (2024)
#### <p align="center"> Uma análise dos padrões de votação nas eleições de São Paulo em 2024, com foco no comportamento do eleitor, abstenção e tendências geográficas.

<br>

📺[Assista  no You Tube](https://youtu.be/NvBFw0Z8X0o)

https://github.com/user-attachments/assets/c34557e8-d1a3-4baa-b995-79b91669b3dd

<br>

#### <p align="center"> [![Patrocine Mindful AI Assistants](https://img.shields.io/badge/Sponsor-Mindful%20AI%20%20Assistants-brightgreen?logo=GitHub)](https://github.com/sponsors/Mindful-AI-Assistants)

<br>

Este projeto fornece uma análise detalhada dos **padrões de votação** nas eleições municipais de São Paulo de 2024, com foco nos **primeiro e segundo turnos** das corridas para prefeito e vereador. Ele examina aspectos chave como **comportamento do eleitor**, **mudanças entre os turnos** e **variações regionais na participação eleitoral**.

**O conjunto de dados foi [***compilado manualmente a partir de fontes oficiais***]()**, inclui mais de **15.000 entradas**. Para coletar dados relevantes, o projeto utilizou técnicas de **web scraping**, seguidas de **limpeza de dados** e **análise exploratória de dados (EDA)**. Esses métodos revelam insights valiosos sobre tendências eleitorais e fornecem **orientações estratégicas** para entender a dinâmica política de São Paulo, o que pode informar **estratégias eleitorais futuras**.

Este trabalho foi desenvolvido como parte do curso **Projeto Integrado e Storytelling** no segundo semestre do curso de **Ciência de Dados e Inteligência Artificial** na **PUC-SP** em 2024, sob a mentoria do renomado professor [✨ Rooney Ribeiro Albuquerque Coelho](https://www.linkedin.com/in/rooney-coelho-320857182/)

Sua **experiência** e **dedicação inabalável** ao ensino desempenharam um papel crucial em aprofundar nosso entendimento tanto da **ciência de dados** quanto da **arte de contar histórias**.

<br><br>  

<!--  INÍCIO DO CORPO  -->

## [Mapa Interativo]() 

<p align="center">
Clique no mapa abaixo para acessar o mapa completo:
</p>

<p align="center">
  <a href="https://github.com/Mindful-AI-Assistants/SP2024-Election-Analysis/blob/1b651c5bfe8633a6324c4d3ed69fc1bac984c3b9/Maps/bairros.json" />
    <img src="https://github.com/user-attachments/assets/54e83b3b-a875-4d76-bcfd-e562c2c12b3c" alt="Map Preview" />
  </a>
</p>

#

## Índice

- [Introdução](#introdução)
- [Objetivos do Estudo](#objetivos-do-estudo)
- [Fundamentação Teórica](#fundamentação-teórica)
- [Descrição do Conjunto de Dados](#descrição-do-conjunto-de-dados)
- [Metodologia](#metodologia)
- [Análise Exploratória de Dados](#análise-exploratória-de-dados)
- [Gráficos e Dashboards](#gráficos-e-dashboards)
  - [7.1. Distribuição de Votos por Município](#71-distribuição-de-votos-por-município)
  - [7.2. Candidatos a Prefeito Mais Votados](#72-candidatos-a-prefeito-mais-votados)
  - [7.3. Candidatos a Vereador Mais Votados](#73-candidatos-a-vereador-mais-votados)
  - [7.4. Prefeitos Mais Votados por Zona Eleitoral](#74-prefeitos-mais-votados-por-zona-eleitoral)
  - [7.5. Vereadores Mais Votados por Zona Eleitoral](#75-vereadores-mais-votados-por-zona-eleitoral)
  - [7.6. Prefeitos Mais Votados por Município](#76-prefeitos-mais-votados-por-município)
  - [7.7. Vereadores Mais Votados por Município](#77-vereadores-mais-votados-por-município)
  - [7.8. Distribuição de Votos por Partido Político](#78-distribuição-de-votos-por-partido-político)
- [Dashboards Interativos](#dashboards-interativos)
  - [8.1. Dashboard 1: Visão Geral dos Votos por Município](#81-dashboard-1-visão-geral-dos-votos-por-município)
  - [8.2. Dashboard 2: Análise dos Candidatos a Prefeito](#82-dashboard-2-análise-dos-candidatos-a-prefeito)
  - [8.3. Dashboard 3: Visão Geral dos Candidatos a Vereador](#83-dashboard-3-visão-geral-dos-candidatos-a-vereador)
  - [8.4. Dashboard 4: Tendências de Votação por Partido e Região](#84-dashboard-4-tendências-de-votação-por-partido-e-região)
  - [8.5. Dashboard 5: Distribuição Geográfica dos Votos](#85-dashboard-5-distribuição-geográfica-dos-votos)
- [Conclusão](#conclusão)
- [Material Extra](#material-extra)
- [Referências](#referências)
- [Como Rodar o Projeto](#como-rodar-o-projeto)
- [Contribuindo](#contribuindo)
- [Nossa Equipe](#nossa-equipe)


## 1. Introdução
     
Este relatório apresenta uma análise detalhada dos dados das eleições municipais de São Paulo de 2024, com foco na distribuição dos votos, comportamento dos eleitores e desempenho dos candidatos a prefeito e vereador. Diversas visualizações e dashboards são utilizados para explorar os padrões de votação, tendências emergentes e os fatores que influenciam os resultados eleitorais.


## 2. Objetivos do Estudo

O estudo tem como objetivo entender a dinâmica eleitoral nas áreas urbanas e periféricas de São Paulo, identificando os fatores que determinam as preferências dos eleitores, como os partidos mais votados, os perfis dos candidatos e o comportamento de voto.


## 3. Fundamentação Teórica
Analisar dados eleitorais é crucial para entender o comportamento do eleitor, as preferências partidárias e as tendências políticas nas diferentes regiões. A visualização de dados oferece uma maneira clara e eficiente de identificar padrões que podem informar campanhas futuras.


## 4. Descrição do Conjunto de Dados
   
Os dados usados neste estudo foram extraídos de fontes públicas, fornecendo informações sobre votos por município, zona eleitoral e partido político. O conjunto de dados inclui detalhes sobre os candidatos a prefeito e vereador em São Paulo, incluindo o número de votos recebidos por cada candidato.

### Os seguintes arquivos CSV foram processados:

- `address_Mayor.csv`
- `Mayor_by_city.csv`
- `Mayor_by_city_round_2.csv`
- `Mayor.csv`
- `address_Councilor.csv`
- `Councilor_by_city.csv`
- `councilor.csv`

### Estrutura das Colunas

Aqui está uma visão geral das principais colunas nos arquivos CSV processados:

- **`NM_MUNICIPIO`**: Nome do município  
- **`NR_ZONA`**: Número da zona eleitoral  
- **`DS_CARGO_PERGUNTA`**: Cargo eleitoral (Prefeito ou Vereador)  
- **`NM_VOTAVEL`**: Nome do candidato  
- **`SG_PARTIDO`**: Sigla do partido  
- **`QT_VOTOS`**: Número de votos recebidos  


## 5. Metodologia

A metodologia foi dividida em várias etapas:

- **Pré-processamento de Dados**: Leitura e concatenação dos datasets, limpeza de registros inválidos.
- **Análise Exploratória de Dados (EDA)**: Identificação de padrões e tendências de votação usando gráficos e tabelas.
- **Visualização de Dados**: Criação de gráficos interativos com a biblioteca Plotly para exploração dinâmica dos resultados.


## 6. Análise Exploratória de Dados

A análise exploratória revelou várias tendências interessantes, como:

- A predominância dos votos para partidos como MDB e PSOL.
- Uma distribuição geográfica de votos mostrando alta concentração no centro de São Paulo e maior apoio a partidos progressistas nas áreas periféricas.


## 7. Gráficos e Dashboards
   
### 7.1. Distribuição de Votos por Município

```python
import plotly.express as px
import pandas as pd

# Leitura do dataset
election = pd.read_csv('/path/to/your/data.csv', encoding='latin-1')

# Plotando a distribuição de votos por município
fig = px.histogram(election, x="NM_MUNICIPIO", y="QT_VOTOS", 
                   title="Votos por Município", 
                   color_discrete_sequence=["#1f77b4"])
fig.update_layout(b
```




















## 💌 [Entre em Contato]()

For any questions or suggestions, please feel free to reach out:

- **Fabiana 🚀 Campanari** - [email me](mailto:fabicampanari@proton.me)
- **Fabiana 🚀 Campanari** -[LinkedIn](https://www.linkedin.com/in/fabiana-campanari/)
- **Fabiana 🚀 Campanari** - [Contacts Hub](https://linktr.ee/fabianacampanari)

<br>  

- **Pedro 🛰️  Vyctor** - [email me](mailto:pedro.vyctor00@gmail.com)
- **Pedro 🛰️  Vyctor** -[LinkedIn](https://www.linkedin.com/in/pedro-vyctor-almeida-285b89273?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BJmPKs0gjS4Sqzuw1d2%2FMjg%3D%3D)

 

## [Main Contributors]() 

<br>

- [Fabiana 🚀 Campanari](https://github.com/FabianaCampanari)
- [Pedro 🛰️ Vyctor](https://github.com/ppvyctor)


<br><br>

<p align="center"> <a href="#Top">Back to top</a>

#
 
##### <p align="center">Copyright 2024 Mindful-AI-Assistants. Code released under the  [MIT license.]( https://github.com/Mindful-AI-Assistants/.github/blob/ad6948fdec771e022d49cd96f99024fcc7f1106a/LICENSE)

# <p align="center"> 🗳 Análise da Eleição SP2024 
### <p align="center"> An analysis of voting patterns in São Paulo's 2024 elections, focusing on voter behavior, absenteeism, and geographic trends.📍
 

