# Group 6 ITCS-6162 Food and World Analysis
## Implementation of Exploratory Data Analysis

![Global-food-supply-balance-is-becoming-increasingly-unstable-as-population-grows_wrbm_large](https://user-images.githubusercontent.com/54337476/144952418-cb336eb3-def8-41c3-93db-19e16015e007.jpg)

## Project and Team Introduction:

### Team Members: 
Arvind Suryiakanth  
Calvin Moore  
Ramesh Gururajan  
Roy Ulrichiii

### Project Summary:
In order to cope with the need for food, we need to devise a way to balance supply and demand. For any country, the production of food is influenced by two main factors, natural resources and institutional support. Natural resources include fertile land, forest, water, etc. Institutional resources include local and national government bodies. Our project is going to examine the demand for certain main food sources such as milk, wheat, and soy. from different countries within a given population. Then, we are going to merge this data with expected population growth to see if the countries can sustain using that resource for the growing population or should change to something better suited to the resources available.

### Problem Statement:
For a given economic measure of a country with respect to population 
and production of feed and food, we want to evaluate what are the fastest growing countries and balance the supply and demand based on analysis of economic measures and agricultural production.

## Data and Source description:

### Datasource:
The datasets that we used came from [Kaggle](https://www.kaggle.com/) and [World Bank](https://www.worldbank.org/en/home) for our project. The data for our food came from this page [Food data](https://www.kaggle.com/dorbicycle/world-foodfeed-production). The data for our world population datasets came from this page [Population data](https://data.worldbank.org/indicator/SP.POP.TOTL).

### Introduction to the Dataset:


## CRISP-DM Process:
We have undergone these steps as a part of CRISP-DM:

- [Business understanding](https://github.com/ramkguru97/Group_6_6162#business-understanding)
- [Data Understanding and EDA](https://github.com/ramkguru97/Group_6_6162#data-understanding-and-eda)
- [Data Preparation](https://github.com/ramkguru97/Group_6_6162#data-preparation)
- [Modeling](https://github.com/ramkguru97/Group_6_6162#modeling)
- [Evaluation](https://github.com/ramkguru97/Group_6_6162#evaluation)
- [Deployment](https://github.com/ramkguru97/Group_6_6162#deployment)

## Research understanding:


## Data Understanding and EDA:


## Data Preparation:
1. Merged data from FAO.csv and GlobalPopulation.csv.
2. Merged from csvs put into new dataframe, called "result", on condition Country Name.
3. Created heatmap to show columns with null values.
4. 

## Modeling:
After the data prep phase, we have implemented 
![image](https://user-images.githubusercontent.com/89566244/145322294-58b02a8c-8827-4635-8168-1a3eda65cf90.png)

## Evaluation:
All the models that were built 

## Deployment:

### Conclusion:


### Future Work:
Plans for futhur working on this project would be to obtain more data from different countries we don't already have and to obtain more recent data from the countries we are taking a look at. Once, more data is obtained then more EDA methods will be used to make the mass data collected easier to work with. After that, more visualiztions and models will be implemented to help more people interested in the project undertand the approach we are going for, why this knowlege gathered is important, and what this means for humans if these trends continue.

We can make use the model generated [K-Mean clustering] for any type of dataset [Food/Feed Vs Country : Which we modelled in our project for top 10 countries] having Food Vs countries from each continent , Food Vs Population for any given country or Countries. This will eventually help predict the supply [Food production] Vs Demand [Population growth]. Clusterting the country based on food type[Food production] for a given lattitude-longitude or country location can be leveraged, if surplus, to meet the population growth in different lattitude-longitude or coiuntry location where there is food scarcity. 

### Instructions to Use
To continue work on this project the final notebook and data files included in this github site can be downloaded; and used in Anaconda, Google Colab, or any other python friendly environments that will support jupter notebooks.
