# ValdezKuuskvereAnsbro
ENV 872 Course Project for T. Valdez, C. Kuuskvere, E. Ansbro
# <Repository Title>
<Instructions: copy and paste this template into your project README file (found in the parent folder of the repository). Fill in relevant information as requested.>

<General notes: add as much information as is relevant for your repository. Some overarching guidelines are provided, but feel free to expand on these guidelines.>
<More resources found here: https://www.dataone.org/all-best-practices>
<Delete the text inside the brackets when formatting your file.>

## Summary

<describe the purpose of this repository, the information it contains, and any relevant analysis goals. What, why, where, when, how?>

This repository contains final project work completed for the Duke University Nicholas School of the Environment Fall 2023 Environmental Data Exploration course. The purpose of this repository is to showcase team members Tani Valdez Rivas, Cara Kuuskvere, and Erin Ansbro's environmental data analytics skills in R studio through an investigation of Nitrogen Surge Uptake in Giant Kelp through an evaluation of a data set from the Environmental Data Initiative Repository. We evaluate data from the Santa Barbara Coastal LTER Reef: Surge uptake capability in Macrocystis pyrifera in response to pulses of three different forms of nitrogen (doi:10.6073/pasta/d079ff0e95defb71b87040f56235d755). We aim to answer four proposed research questions regarding which variables in the data sets influence Nitrogen Surge Uptake Rates. This evaluation is conducted through data wrangling, exploration by means of mapping the samples and visualizing variables with box and violin plots, and analysis conducted by means of data visualization and statistical anova, linear regression, and tukey HSD tests.  

## Investigators
Erin Ansbro, Duke University Nicholas School of the Environment
Master of Environmental Management Candidate Class of 2025
Environmental Data Analytics Fall 2023 Student 
erin.ansbro@ duke.edu 

Cara Kuuskvere, Duke University Nicholas School of the Environment
Master of Environmental Management Candidate Class of 2025
Environmental Data Analytics Fall 2023 Student 
cara.kuuskvere@ duke.edu 

Tani Valdez Rivas, Duke University Nicholas School of the Environment
Master of Environmental Management Candidate Class of 2025
Environmental Data Analytics Fall 2023 Student 
Tani.ValdezRivas@ duke.edu 



## Keywords

Giant Kelp, EDEFall2023, Nitrogen Surge Uptake, Duke University Nicholas School, SBC LTER, Time Series Analysis, Data Visualization, Season, Nitrogen Types (ammonia, nitrate, urea)
<add relevant keywords here>

## Database Information

<describe the origin of all data in the repository, including data collected from outside sources and new data generated by the investigator(s). If data was accessed from an outside database, the date(s) of data access should also be included.>
Processed and raw

## Folder structure, file formats, and naming conventions 

<describe the folders contained in the repository, including what type of files they contain>
Code: r-markdown files containing data processing and wrangling code, data exploration, data analysis, and the project report r-markdown and HTLM files. 

Data:
  Processed: exported csv files resulting from data wrangling and processing 
  Raw: imported csv files from environmental data initiative 
  
Output: 
  BoxDataExp: PNG files of box plots created to visualize variables' mean and quartiles in the data exploration component of our work
    naming convention: variable measured, visualization type, variable measured against 
  ViolinDataExp: PNG files of violin plots created to visualize variables' range and spread in the data exploration component of our work
    naming convention: variable measured, visualization type, variable measured against
  Analysis: PNG files of box and scatter plots resulting from data visualizations produced to supplement analysis of research questions.
  naming convention: variable measured, variable measured against, visualization type [CHANGE]
<describe the formats of files for the various purposes contained in the repository>

<describe your file naming conventions>

## Metadata

<For each data file in the repository, describe the data contained in each column. Include the column name, a description of the information, the class of data, and any units associated with the data. Create a list or table for each data file.> 

details on every CSV file

## Scripts and code


explain purpose of each code file and packages in each
<list any software scripts/code contained in the repository and a description of their purpose.>

## Quality assurance/quality control
removing NAs, cleaning, wrangling....

<describe any relevant QA/QC procedures taken with your data. Some ideas can be found here:>
<https://www.dataone.org/best-practices/develop-quality-assurance-and-quality-control-plan>
<https://www.dataone.org/best-practices/ensure-basic-quality-control>
<https://www.dataone.org/best-practices/communicate-data-quality>
<https://www.dataone.org/best-practices/identify-outliers>
<https://www.dataone.org/best-practices/identify-values-are-estimated>