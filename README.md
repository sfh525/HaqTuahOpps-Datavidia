# Food Commodity Time Series Price Prediction

## Credits
Credits goes to my teammates for contributing to this project: 
1. Tristan Khayru Abiyudha
2. Daniel Winston Mandela Tulung

## Intro
The competition presented a challenge of predicting the price of multiple food commodities for an extended period of time (around 3 months). Prediction is supposed to be done for all provinces in Indonesia.

## Dataset
The dataset was large. Various data was provided such as the price of the food commodities for around 2 years, money exchange data, global commodity prices, and Google trend's search data for each commodity for each region. 
It is important to note that the food commodity data had columns of prices for every province in Indonesia. As for the test sample, it only contained placeholder values of 0's, no data for the 
calculate from. 

## Approach
Our final approach trained a model for every specific commodity, for every specific region. In total, there are 442 models. The 2 models that proved to be effective were ExtraTrees and KNN. However, despite the large number of models trained, the models were lightweight enough that training did not take long. Each of those models are then tasked to predict the price of each commodity in a given province.  

## Result and Potential Improvements
The model's performance was measured using Mean Absolute Percentage Error (MAPE) metric. Our approach achieved a MAPE score of 0.05198, or ranked #34 out of 229 teams. 

## Runnning the Notebook
This notebook can be run in any environment you would like. Make sure to match the directory of the dataset and install all the necessary dependencies. 
