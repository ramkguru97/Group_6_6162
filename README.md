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
The datasets that we used came from [Kaggle](https://www.kaggle.com/) and [World Bank](https://www.worldbank.org/en/home) for our project. The data for our food came from this page [Food data](https://www.kaggle.com/dorbicycle/world-foodfeed-production). The data specifically focuses on comparison between food produced for human consumption 
and feed produced for animals. The data is collected from The Food and Agriculture Organization of the United Nations for over 245 countries from 1961 to 2013 and consists of 63 columns and 21478 rows. The data for our world population datasets came from this page [Population data](https://data.worldbank.org/indicator/SP.POP.TOTL). The data collected is seperated into population total, population male, population female % of total population male, and % of total population female. This data is collected from 245 countries from 1960-2020.

## CRISP-DM Process:
We have undergone these steps as a part of CRISP-DM:

- [Business understanding](https://github.com/ramkguru97/Group_6_6162#business-understanding)
- [Data Understanding and EDA](https://github.com/ramkguru97/Group_6_6162#data-understanding-and-eda)
- [Data Preparation](https://github.com/ramkguru97/Group_6_6162#data-preparation)
- [Modeling](https://github.com/ramkguru97/Group_6_6162#modeling)
- [Evaluation](https://github.com/ramkguru97/Group_6_6162#evaluation)
- [Deployment](https://github.com/ramkguru97/Group_6_6162#deployment)

## Research understanding:
Our world population is expected to grow from 7.3 billion today to 9.7 billion in the year 2050. Finding solutions for feeding the growing world population has become a hot topic for food and agriculture organizations. These solutions range from changing the way we grow our food to changing the way we eat. The food dataset is focused on two utilizations of each food item available:  
  Food - refers to the total amount of the food item available as human food during the reference period.  
Feed - refers to the quantity of the food item available for feeding to the livestock and poultry during the reference period.

### Research Focus Areas:
-Top Foods Produced  
-Percentage Analysis Feed vs Food  
-Top Markets Contributing Towards Specific Food Production  
-Grouping of Specific Items  
-Unique Countries Food/Feed Production for Given Year

## Data Understanding and EDA:
This displays the overall count between Food and Feed and generates category plot based on the ELement 
![image](https://user-images.githubusercontent.com/54337476/145330618-4db32094-2401-4374-a68b-803ceeaf0320.png)

Feed and food production plot - pie chart
![image](https://user-images.githubusercontent.com/54337476/145330777-0da6bce1-772b-442d-8c03-42321a46e1f9.png)

Factor plot to show the count of all the items produced inclusive of feed/food
![image](https://user-images.githubusercontent.com/54337476/145330836-7df3b311-1922-4a8a-952b-ec66c7a1ba51.png)

Factorplot --> feed/food production for items oats/spices 
![image](https://user-images.githubusercontent.com/54337476/145330918-60211367-f0f3-4c1f-afe5-57cd2560403e.png)

## Data Preparation:
1. Merged data from FAO.csv and GlobalPopulation.csv.
2. Merged from csvs put into new dataframe, called "result", on condition Country Name.
3. Identifying Missing Values
4. Created heatmap to show columns with null values.
5. Check for Null Values
6. Duplicate Data Check
7. Duplicate Data Dropping
8. Drop Missing Values

## Modeling:
After the data prep phase, we have implemented K-mean Clustering. Since we dont have a target variable, we have to go with unsupervised learing. As a part of the same we implemented K-mean cluster in order to find a optimal centriods [See image below, its Item Code Vs Country Code(latitude-longitude]. The optimal centriod [shown in Red dot] is the position of latitude-longitude [or]Country location where that particular food item produced in surplus. 
![image](https://user-images.githubusercontent.com/89566244/145322294-58b02a8c-8827-4635-8168-1a3eda65cf90.png)

## Evaluation:
As as a result of our model using K-means clustering which  is a machine learning clustering technique used to simplify large datasets into smaller and simple datasets. [From 20,000 or more records plus merging food & population dataset] Distinct patterns are evaluated and similar data sets are grouped together. The variable K represents the number of groups in the data. With the model we are able to come up with optimal groups of different food types for any given cluster of countries,  which can be leveraged for future work. K-mean is easy to implement and identify unknown groups of data from complex data sets. The  results are presented in an easy and simple manner.  

## Deployment:

### Conclusion:
We can make use the model generated [K-Mean clustering] for any type of dataset [Food/Feed Vs Country : Which we modelled in our project for top 10 countries] having Food Vs countries from each continent , Food Vs Population for any given country or Countries. This will eventually help predict the supply [Food production] Vs Demand [Population growth]. Clusterting the country based on food type[Food production] for a given lattitude-longitude or country location can be leveraged, if surplus, to meet the population growth in different lattitude-longitude or coiuntry location where there is food scarcity.

### Future Work:
Plans for futhur working on this project would be to obtain more data from different countries we don't already have and to obtain more recent data from the countries we are taking a look at. Once, more data is obtained then more EDA methods will be used to make the mass data collected easier to work with. After that, more visualiztions and models will be implemented to help more people interested in the project undertand the approach we are going for, why this knowlege gathered is important, and what this means for humans if these trends continue.

### Instructions to Use
To continue work on this project the final notebook and data files included in this github site can be downloaded; and used in Anaconda, Google Colab, or any other python friendly environments that will support jupter notebooks.
