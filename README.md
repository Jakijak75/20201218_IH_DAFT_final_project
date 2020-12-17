# 20201218_IH_DAFT_final_project

### "Life expectancy inequality around the globe and factors influencing it"

### 1.	Initial project scope

The goal of this project is to analyze life expectancy values in countries across the globe from a static and dynamic point of view and answer the following questions:
•	How has life expectancy been evolving across countries in the past 25 years?
•	What are the factors that have the most impact on life expectancy in a country?
•	Which national and cross-national policies should be implemented in order to increase life expectancy in countries lagging behind?

To achieve this, the idea is to run multiple linear regressions on a set of data which is large enough to be significant, and which links average life expectancy to other data.

### 2.	The challenge of data quality

The best dataset candidate for this project was the one available on Kaggle: https://www.kaggle.com/kumarajarshi/life-expectancy-who

It has a silver medal and is referenced on multiple website and machine learning forums.

However, upon closer consideration, the data quality of this dataset was unsatisfactory. 

In addition to lacking sources and insufficient data description, some sanity check revealed some major inconsistencies. 

This slightly modified the scope of the project, as the main focus of the jupyter notebook became to assess the quality of the data through code and clean it whenever possible. 

### 3.	Building a new time series dataset

As the initial dataset proved unusable, I decided to rebuild one from scratch, using mainly the data aggregated by gapminder (https://www.gapminder.org/data/) and trying to select the most relevant datasets. 

The main difficulty here (in addition to manipulating and aggregating 10+ datasets) was to pay very close attention to the methodology of data collection over time, and to select the relevant timeframe over which data collection methods remained consistent

### 4.	Outcome

The data collected allowed to run accurate regression models, with an R2 of 0.9+ and statistical significance for most variables used.
Next steps include:
-	Automating the replacing of NaN-values in the dataframe
-	Adding more relevant variables
-	Answering the initial question regarding which policies would be most efficient for a given groups of countries in order to increase life expectancy

### 5.	Repo structure – self-explanatory
