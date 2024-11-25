<br>

 \[[🇧🇷 Português](README.pt_BR.md)\] \[**[🇺🇸 English](README.md)**\]

<br>

  <!--  START HEADER  -->
## <p align="center">    📊 Data Analysis and Visualization: São Paulo Municipal Elections  - 1st and 2nd Round (2024)
#### <p align="center">  An analysis of voting patterns in São Paulo's 2024 elections, focusing on voter behavior, absenteeism, and geographic trends.

<br>

https://github.com/user-attachments/assets/1b17d66f-3fa0-40dc-bfdc-031ca5b703aa

 <br>

 #### <p align="center"> [![Sponsor Mindful AI Assistants](https://img.shields.io/badge/Sponsor-Mindful%20AI%20%20Assistants-brightgreen?logo=GitHub)](https://github.com/sponsors/Mindful-AI-Assistants)

 <br>

This project provides an in-depth analysis of **voting patterns** in the 2024 São Paulo municipal elections, with a focus on the **first and second rounds** of mayoral and city council races. It examines key aspects such as **voter behavior**, **shifts between rounds**, and **regional variations in voter turnout**. 

**The dataset was [***manually compiled from official sources***]()** , includes over **15,000 entries**. To gather relevant data, the project employed **web scraping** techniques, followed by **data cleaning** and **exploratory data analysis (EDA)**. These methods uncover valuable insights into electoral trends and provide **strategic guidance** for understanding the political dynamics of São Paulo, which can inform **future election strategies**


This work was developed as part of the **Integrated Project and Storytelling** course in the second semester of the undergraduate program in **Data Science and Artificial Intelligence** at **PUC-SP** in 2024, under the mentorship of the renowned  Professor [✨ Rooney Ribeiro Albuquerque Coelho](https://www.linkedin.com/in/rooney-coelho-320857182/) 

His **expertise** and **unwavering dedication** to teaching played a crucial role in deepening our understanding of both **data science** and the **art of storytelling**.


 <br><br>  

<!--  START BODY  -->

## [Interactive Map]() 

<p align="center">
To access the full Map, click the Map below:
</p>

<p align="center">
  <a href="https://github.com/Mindful-AI-Assistants/SP2024-Election-Analysis/blob/1b651c5bfe8633a6324c4d3ed69fc1bac984c3b9/Maps/bairros.json" />
    <img src="https://github.com/user-attachments/assets/54e83b3b-a875-4d76-bcfd-e562c2c12b3c" alt="Map Preview" />
  </a>
</p>


#

## Table of Contents

- [Introduction](#introduction)
- [Study Objectives](#study-objectives)
- [Theoretical Background](#theoretical-background)
- [Dataset Description](#dataset-description)
- [Methodology](#methodology)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Charts and Dashboards](#charts-and-dashboards)
  - [7.1. Vote Distribution by Municipality](#71-vote-distribution-by-municipality)
  - [7.2. Most Voted Mayoral Candidates](#72-most-voted-mayoral-candidates)
  - [7.3. Most Voted Councilor Candidates](#73-most-voted-councilor-candidates)
  - [7.4. Most Voted Mayors by Electoral Zone](#74-most-voted-mayors-by-electoral-zone)
  - [7.5. Most Voted Councilors by Electoral Zone](#75-most-voted-councilors-by-electoral-zone)
  - [7.6. Most Voted Mayors by Municipality](#76-most-voted-mayors-by-municipality)
  - [7.7. Most Voted Councilors by Municipality](#77-most-voted-councilors-by-municipality)
  - [7.8. Vote Distribution by Political Party](#78-vote-distribution-by-political-party)
- [Interactive Dashboards](#interactive-dashboards)
  - [8.1. Dashboard 1: Overview of Votes by Municipality](#81-dashboard-1-overview-of-votes-by-municipality)
  - [8.2. Dashboard 2: Mayoral Candidates Analysis](#82-dashboard-2-mayoral-candidates-analysis)
  - [8.3. Dashboard 3: Councilor Candidates Overview](#83-dashboard-3-councilor-candidates-overview)
  - [8.4. Dashboard 4: Voting Trends by Party and Region](#84-dashboard-4-voting-trends-by-party-and-region)
  - [8.5. Dashboard 5: Geographic Distribution of Votes](#85-dashboard-5-geographic-distribution-of-votes)
- [Conclusion](#conclusion)
- [Extra Material](#extra-material)
- [References](#references)
- [How to Run the Project](#how-to-run-the-project)
- [Contributing](#contributing)
- [Our Team](#our-team)


 ## 1. Introduction
     
This report presents a detailed analysis of the data from São Paulo's 2024 municipal elections, focusing on vote distribution, voter behavior, and the performance of mayoral and councilor candidates. Various visualizations and dashboards are used to explore voting patterns, emerging trends, and the factors influencing electoral outcomes.


## 2. Study Objectives

The study aims to understand electoral dynamics in São Paulo's urban and peripheral areas, identifying factors determining voter preferences, such as the most-voted parties, candidate profiles, and voting behavior.


## 3. Theoretical Background
Analyzing electoral data is crucial for understanding voter behavior, party preferences, and political trends across different regions. Data visualization offers a clear and efficient way to identify patterns that can inform future campaigns.


## 4. Dataset Description
   
The data used in this study were extracted from public sources, providing information on votes by municipality, electoral zone, and political party. The dataset includes details about mayoral and councilor candidates in São Paulo, including the number of votes received by each candidate.

### The following CSV files were processed:

address_Mayor.csv
Mayor_by_city.csv
Mayor_by_city_round_2.csv
Mayor.csv
address_Councilor.csv
Councilor_by_city.csv
councilor.csv
Sample column structure:
NM_MUNICIPIO: Municipality name
NR_ZONA: Electoral zone number
DS_CARGO_PERGUNTA: Election role (Mayor or Councilor)
NM_VOTAVEL: Candidate name
SG_PARTIDO: Party acronym
QT_VOTOS: Number of votes received

### Processed Files

The following CSV files were processed:

- `address_Mayor.csv`
- `Mayor_by_city.csv`
- `Mayor_by_city_round_2.csv`
- `Mayor.csv`
- `address_Councilor.csv`
- `Councilor_by_city.csv`
- `councilor.csv`



### Sample Column Structure

Here is an overview of the main columns in the processed CSV files:

- **`NM_MUNICIPIO`**: Municipality name  
- **`NR_ZONA`**: Electoral zone number  
- **`DS_CARGO_PERGUNTA`**: Election role (Mayor or Councilor)  
- **`NM_VOTAVEL`**: Candidate name  
- **`SG_PARTIDO`**: Party acronym  
- **`QT_VOTOS`**: Number of votes received  


## 5. Methodology

The methodology was divided into several steps:

- **Data Preprocessing**: Reading and concatenating datasets, cleaning invalid records.
- **Exploratory Data Analysis (EDA)**: Identifying voting patterns and trends using graphs and tables.
- **Data Visualization**: Creating interactive charts with the Plotly library for dynamic result exploration.


## 6. Exploratory Data Analysis

The exploratory analysis uncovered several interesting trends, such as:

- The dominance of votes for parties like MDB and PSOL.
- A geographic vote distribution showing high concentration in central São Paulo and greater support for progressive parties in peripheral areas.


## 7. Charts and Dashboards
   
### 7.1. Vote Distribution by Municipality

```python
import plotly.express as px
import pandas as pd

# Reading the dataset
election = pd.read_csv('/path/to/your/data.csv', encoding='latin-1')

# Plotting vote distribution by municipality
fig = px.histogram(election, x="NM_MUNICIPIO", y="QT_VOTOS", 
                   title="Votes by Municipality", 
                   color_discrete_sequence=["#1f77b4"])
fig.update_layout(bargap=0.2)
fig.show()
```

<br>

<p align="center">
 <img src="https://github.com/user-attachments/assets/78431749-1bcc-449a-8876-0991b9a4bace"/>

<br>











<!--

###  Power BI [Dashboard Access Link](https://app.powerbi.com/view?r=eyJrIjoiNTNmY2Y2YzgtODY3Yy00M2ViLWI0NDItMTdiZDJlNTg4Zjk2IiwidCI6IjhlYjI5MjAxLWEyN2QtNDMwMi04NDczLWM5ODJlYjViZTkzNSJ9
)


### Power BI QR Code

 <p align="center">  
<img src="https://github.com/user-attachments/assets/dfc4a631-5f88-42ea-8fea-9186beaeffef" />


-->




## Our Team

### 💌 [Contact Us]()

For any questions or suggestions, please feel free to reach out:

- **Fabiana 🚀 Campanari** - [email me](mailto:fabicampanari@proton.me)
- **Pedro 🛰️  Vyctor** - [email me](mailto:pedro.vyctor00@gmail.com)
 

## [Main Contributors]() 

- [Fabiana 🚀 Campanari](https://github.com/FabianaCampanari)
- [Pedro 🛰️ Vyctor](https://github.com/ppvyctor)


<br><br>

<p align="center"> <a href="#Top">Back to top</a>

#
 
##### <p align="center">Copyright 2024 Mindful-AI-Assistants. Code released under the  [MIT license.]( https://github.com/Mindful-AI-Assistants/.github/blob/ad6948fdec771e022d49cd96f99024fcc7f1106a/LICENSE)
