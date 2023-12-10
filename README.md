# ValdezKuuskvereAnsbro
ENV 872 Course Project for T. Valdez, C. Kuuskvere, E. Ansbro
# ValdezKuuskvereAnsbro

## Summary
This repository contains final project work completed for the Duke University Nicholas School of the Environment Fall 2023 Environmental Data Exploration course. The purpose of this repository is to showcase team members Tani Valdez Rivas, Cara Kuuskvere, and Erin Ansbro's environmental data analytics skills in R studio through an investigation of Nitrogen Surge Uptake in Giant Kelp through an evaluation of a data set from the Environmental Data Initiative Repository. We evaluate data from the Santa Barbara Coastal LTER Reef: Surge uptake capability in Macrocystis pyrifera in response to pulses of three different forms of nitrogen (doi:10.6073/pasta/d079ff0e95defb71b87040f56235d755) as well as a temporal documentation of this dataset for time series analysis. We aim to answer five proposed research questions regarding which variables in the data sets influence Nitrogen Surge Uptake Rates and to analyze the temporal elements of nitrogen uptake rate. This evaluation is conducted through data wrangling, exploration by means of mapping the samples and visualizing variables with box and violin plots, and analysis conducted by means of data visualization and statistical anova, linear regression, and tukey HSD tests.  

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

## Database Information


Nitrogen (Raw): SBC LTER: Reef: Surge uptake capability in Microcystis pyrifera in response to pulses of three different forms of nitrogen. Accessed November 15, 2023 from environmental data initiative digital repository. doi:10.6073/pasta/d079ff0e95defb71b87040f56235d755

Nitrogen (Processed): Investigator cleaned and processed data from nitrogen raw data source. 

Nitrogen Years (Raw): SBC LTER: Santa Barbara Coastal LTER, Reed, D., Miller, R. (2021). SBC LTER: Reef: Macrocystis pyrifera CHN content (carbon, hydrogen, nitrogen), ongoing since 2002 ver 21. Environmental Data Initiative. https://doi.org/10.6073/pasta/48686fef076a23310a0e48f69d76260c (Accessed 2023-11-27).

Nitrogen Years (Processed): Investigator cleaned and processed data from nitrogen years raw data source

## Folder structure, file formats, and naming conventions 

Code: r-markdown files containing data processing and wrangling code, data exploration, data analysis, and the project report r-markdown and HTLM files. 

Data:
  Processed: exported csv files resulting from data wrangling and processing 
  Raw: imported csv files from environmental data initiative 
  
Output: 
Exploratory Analysis: PNG files of time series point plots to visualize temporal data 
    naming convention: variable measured, visualization type, variable measured against 
 BoxDataExp: PNG files of box plots created to visualize variables' mean and quartiles in the data exploration component of our work
    naming convention: variable measured, visualization type, variable measured against 
  ViolinDataExp: PNG files of violin plots created to visualize variables' range and spread in the data exploration component of our work
    naming convention: variable measured, visualization type, variable measured against
  Analysis: PNG files of box and scatter plots resulting from data visualizations produced to supplement analysis of research questions.
  naming convention: variable measured, variable measured against, visualization type 


## Metadata

Raw
Nitrogen: CSV file containing 359 rows and 9 columns
Columns: nitrogen species (factor), season (factor), day replicate (int), time (int), blade replicate (int), nitrogen uptake rate (number)(1/ min), biomass normalized uptake rate (number) (micrograms per gram per min), final percent nitrogen (number), initial percent nitrogen (number)

NitrogenYears: CSV file containing 1334 rows and 16 columns
Columns: CONSEC (int), year (int), month (int), date selected (factor), site (factor), X Nitrogen (int), replicate (int), wet weight (number), dry weight (number), dry versus wet ratio (number), analyzed weight (int), carbon (number), hydrogen (number), nitrogen (number), carbon nitrogen ration (number), experiment notes (factor)

Processed: 
Nitrogen: CSV file containing 359 rows and 9 columns 
Columns: nitrogen species (factor), season (factor), day replicate (factor), time (factor), blade replicate (factor), nitrogen uptake rate (number) (1/min), biomass normalized uptake rate (number)(micrograms per gram per min), final percent nitrogen (number), initial percent nitrogen (number); with data cleaned to reflected needed variable data structures


NitrogenYears: CSV file containing 1289 rows and 17 columns
Columns: sample number (int), year (int), month (int), full date (date), site (factor), number of samples (int), sample replicate (int), wet weight (number), dry weight (number), ratio dry to wet weight (number), analytical dry weight (int), carbon percent (number), hydrogen percent (number), nitrogen percent (number), carbon to nitrogen ratio (number), notes (factor), and new site name (factor); with cleaned and processed data and clean data structures for analysis 


## Scripts and code
DataProcessingandWrangling
In this code file, we import our raw dataset and clean the file in order to best use it for our exploration and analysis. We transform some of the data into factors to analyze our information and properly process the time components of our dataset. 
Packages: 
-	Here
-	Tidyverse
-	Lubridate

DataExploration
This code file contains data visualization and summary statistics of our dataset after we imported and cleaned. It creates output files for boxplots and violin plots to better understand the data we are working with. 
Packages: 
-	Tidyverse 
-	Lubridate
-	SF
-	Leaflet
-	mapview

DataAnalysis.Rmd
This code file contains our data analysis to answer our research questions. 
Packages: 
-	Tidyverse
-	Lubridate
-	Cowplot
-	Agricolae
-	Sf
-	Leaflet 
-	Mapview
-	Forcats

ValdezKuuskvereAnsbroENV872Project
This code file contains our final project submission. It shows our data wrangling process, data exploration, hypothesis testing, and analysis conducted with our Kelp dataset. It brings together individual work completed in our other code finals to create our final project document. 
Packages: 
-	Tidyverse 
-	Lubridate
-	Cowplot
-	Knitr
-	Sf
-	Leaflet
-	Mapview
-	Here

## Quality assurance/quality control

We conducted quality assurance and controls of our dataset through our data wrangling and cleaning process. In our data wrangling, we converted the datatypes of our variables to factors, integers, and data data types as needed. We also controlled our data by screening for and removing N/As and applying proper time series evaluation against our temporal dependent data. Further, we explored our datasets using box and violin plots to understand their means and ranges and screen for outliers that may skew our datasets. 
