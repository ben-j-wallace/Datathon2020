# Datathon2020

### Team bAESIAN statistics: Albert Sun, Ben Wallace, Larry Zheng, and Lily Zhu 

## Background

The COVID-19 pandemic has changed virtually every facet of our lives. As the months continue to pass by, we are finally beginning to witness and understand the devastating long-term economic implications of this pandemic and the various shutdowns that it has necessitated. In this Datathon, teams will be tasked with using a data-driven approach to answer the following question: which cities around the world will feel the economic impact of COVID-19 most acutely over the next 1, 2, and 5 years? 

## Abstract

The COVID-19 pandemic and the resulting social distancing measures have drastically changed our daily lives, having a significant economic impact. We investigated various socioeconomic factors as possible predictors of differences in unemployment at the county level across the United States as a result of the pandemic. Through backwards selection analysis of variables from movement trends, unemployment, education, and poverty data, we found average movement for retail, grocery, and workplaces to be the strongest predictors for unemployment rates. Furthermore, we found that the effect of retail grocery  on change in unemployment depends on average grocery movement. By monitoring movement rates and consumer spending in these areas, we could identify and predict future areas of high unemployment.

## Solution

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
  
