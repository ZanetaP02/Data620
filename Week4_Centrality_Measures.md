# Week 4 Assignment: Centrality Measures

**Zaneta Paulusova**  
**DATA 620: Network Analysis and Visualization**

For this assignment, I selected the **All Natural Disasters 1900–2021 (EM-DAT/EOSDIS)** dataset from Kaggle. This dataset contains records of natural disasters from around the world between 1900 and 2021, including floods, storms, earthquakes, droughts, wildfires, and other disaster events. It includes information such as country, continent, year, disaster type, deaths, affected population, and economic damages. The specific file I plan to use is **1900_2021_DISASTERS.xlsx - emdat data.csv**, which contains disaster records for countries across Africa, Asia, Europe, the Americas, and Oceania.

**Dataset Website:**  
[All Natural Disasters 1900–2021 (EM-DAT/EOSDIS)](https://www.kaggle.com/datasets/brsdincer/all-natural-disasters-19002021-eosdis)

Although the dataset is not already organized as a network, it can be converted into one. In my proposed network, each node would represent a **country**. Two countries would be connected if they experienced the same type of disaster during the same year. For example, if two countries both experienced a flood in 2010, they would be connected. The categorical variable for each node would be the country's **continent** (Africa, Asia, Europe, the Americas, or Oceania).

To prepare the data, I would download the dataset from Kaggle and load it into Python using Pandas. I would keep the country, continent, year, and disaster type fields. Next, I would use NetworkX to create the network and calculate degree centrality for each country. Finally, I would compare the degree centrality scores across continents.

A possible outcome of this analysis is that countries with higher degree centrality may also have a larger number of people affected by disasters. Countries that frequently experience common disasters, such as floods and storms, may be connected to more countries and therefore have higher centrality scores. By comparing degree centrality across continents, I may find that some regions are more connected through shared disaster experiences than others.

In conclusion, the **All Natural Disasters 1900–2021 (EM-DAT/EOSDIS)** dataset is a good choice for this assignment because it includes a clear categorical variable, continent, and can be converted into a country-level network. Comparing degree centrality across continents may provide useful insights into how countries are connected through shared disaster experiences and whether those connections relate to disaster impacts. This topic is also related to my interest in studying global natural disasters.

## Reference

Dincer, B. (n.d.). *All Natural Disasters 1900–2021 (EM-DAT/EOSDIS)*. Kaggle. Retrieved from [All Natural Disasters 1900–2021 Dataset](https://www.kaggle.com/datasets/brsdincer/all-natural-disasters-19002021-eosdis).
