# Datathon2020

### Team Baesian statistics: Albert Sun, Ben Wallace, Larry Zheng, and Lily Zhu 

## Background

The COVID-19 pandemic has changed virtually every facet of our lives. As the months continue to pass by, we are finally beginning to witness and understand the devastating long-term economic implications of this pandemic and the various shutdowns that it has necessitated. In this Datathon, teams will be tasked with using a data-driven approach to answer the following question: which cities around the world will feel the economic impact of COVID-19 most acutely over the next 1, 2, and 5 years? 

## Abstract

The COVID-19 pandemic and the resulting social distancing measures have drastically changed our daily lives, especially our economic well-being. We investigated movement trends and various socioeconomic factors to predict differences in unemployment at the county level across the United States during the pandemic. Through backwards selection analysis of variables from movement trends, unemployment, education, and poverty data, we found average movement for retail, grocery, and workplaces to be the strongest predictors for unemployment rates. Furthermore, we found that a significant interaction effect existed between average retail movement and average grocery movement. By monitoring movement rates and consumer spending in these areas, we could identify and predict areas of high unemployment.

## Introduction

Our lives have changed drastically since the onset of the COVID-19 pandemic, and social distancing measures have resulted in shifts in working and spending habits. This has had a profound economic impact, changing job dynamics  across the world (Gharehgozli 2020). The effects of the pandemic on jobs are felt unequally across different regions of the United States. Our team sought to investigate which socioeconomic factors could serve as predictors of unemployment during the COVID-19 pandemic.

## Objectives

+ **Understanding the relationship between movement and county-level unemployment during the COVID-19 pandemic:** How does movement in retail, workplace, and grocery spaces relate to unemployment?  

+ **Predict future shifts in unemployment based on previous data:** Using conclusions from part A, how do we expect unemployment to change in the future, given current trends in movement/mobility? Which developments have remained stable throughout the course of the pandemic and are likely to continue? Which counties will see the most significant increases or decreases in unemployment?

## Methodolgy

- We selected 7 variables we believed to be likely predictors of unemployment_change: `retail_avg`, `grocery_avg` , `workplaces_avg`, `residential_avg` , `medhhinc_2018`, `pct_bachelor_or_higher`, and `pctpovall_2018`.

- Through **backwards selection**, we found retail_avg, grocery_avg, and workplaces_avg to be significant predictors  (p < 0.05).  All else held constant, for each 1% increase in retail_avg, grocery_avg, or workplaces_avg, the unemployment rate is predicted to decrease by 0.073, 0.015, and 0.035, respectively.

- Through a **nested F-test**, we found the interaction term between retail_avg and grocery_avg to be significant, meaning the effect of retail_avg on the unemployment rate depends on grocery_avg.

## Components

### `data` **folder**
  - Description: includes .csv and other data files used in data analysis
  - Files:
### `r` **folder**
  - Description: includes .rmd and other .r files
  - Files
### `output` **folder**
  - Description: includes .pdf knitting and other visualizations
  - Files:
  
