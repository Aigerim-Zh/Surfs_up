# Surfs_up

# Overview of the Analysis
In this project, I am tasked with running weather analysis for Oahu, Hawaii, to support a business proposal to open a new shop serving surfboards and ice cream to locals and tourists. Specifically, I will analyze temperature data for June and December months, from January 1, 2010, to August 23, 2017. It is useful to conduct further suggested analyses to understand weather patterns and their impact on the shop. 

# Data and Features
* Source: [hawaii.sqlite](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Data/hawaii.sqlite)
* Databases with ```SQLite``` and ```SQLAlchemy```
* Programming Tools: ```Python SQL toolkit (SQLAlchemy)```, ```Object Relational Mapper (ORM)```, ```Pandas```, ```numpy```
* Software: ```Python 3.9.2``` through ```Jupyter Notebook```
* Code: 
    * [SurfsUp_Challenge.ipynb](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Code/SurfsUp_Challenge.ipynb) for the analysis from January 1, 2010, to August 23, 2017.
    * [climate_analysis.ipynb](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Code/climate_analysis.ipynb) for the additional analysis from August 23, 2018, and August 23, 2017.
All SQLite databases are flat files, i.e., they don’t have relationships that connect the data to anything else. As a result, flat files can be stored locally, which will help move quicker through the analysis.


# Results

## Summary Statistics for Temperatures in June and December
![](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Results/June_Sum_Stats.png)
![](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Results/December_Sum_Stats.png)

* The average temperature in June is about 75 F degrees, which is about 4% higher than that in December.
* The median and mean temperatures in both months are very close indicating no extreme weather fluctuations.
* However, there seems to be slightly more variability in temperatures in December than that in June. 

![](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Results/June_Temps_Hist.png)
![](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Results/December_Temps_Hist.png)

The histograms above further confirm these observations. 

# Summary
In general, the weather in Oahu seems suitable for the new surf and ice cream shop. There are no extreme fluctuations in the temperature. The temperature in June is only 4% higher, on average, than that in December. Based on the average temperatures, I would not expect extreme rainfall either. 

## Two Additional Queries
Two additional queries show the number of recordings and average temperature by the station. 
* The number of recordings indicates how active a station is, which is important to know to make sure that our analysis is valid 
* The average temperature is a representative measure as we found no significant fluctuations in the data.

These queries will not only help identify optimal locations based on the average temperature but also ensure that the optimal location is suitably active.
![](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Results/June_by_Station.png)
![](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Results/December_by_Station.png)

## Further Analysis
There is a similar analysis done on the weather data in Oahu: [climate_analysis.ipynb](https://github.com/Aigerim-Zh/Surfs_up/blob/main/Code/climate_analysis.ipynb). It includes precipitation, station, and temperature analysis between August 23, 2016, and August 23, 2017. 

In general, for the analysis for June and December, it will be also useful to look at the summary statistics for precipitation. 