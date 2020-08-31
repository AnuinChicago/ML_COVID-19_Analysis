# ML_COVID-19_Analysis
##LINK to website

## Data Cleaning and Exploration

Data Sets
-Covid-19 Blood Panel Data 
https://www.kaggle.com/einsteindata4u/covid19

-Covid-19 Healthy Diet
https://www.kaggle.com/mariaren/covid19-healthy-diet-dataset

-Covid-19 Data from John Hopkins  
https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series

# Question1 Can you predict the severity of COVID-19 from a full blood panel?

Since the pandemic of COVID-19, the prediction of the disease severeness is a challenge to the whole world. Because early symptoms of COVID-19 infection overlap with many other common respiratory diseases, we decided to use a full blood panel to predict the disease prognosis.
The second part of the analysis came with the background of many research paper have reported that high serum glucose level is associated with worth prognosis in COVID-19 positive patient. We were wondering whether we could use the serum glucose level in our dataset to predict the outcome of COVID-19 infection.
We downloaded the data from Kaggle, followed by cleaning up the data using excel and python. Then, we stored the data in AWS, followed by reading the csv file directly from AWS in the jupyter notebook.

## Machine Learning
We used random forest model to check whether the full blood counts could predict COVID-19 prognosis in patients, while logistic regression model was used to test the correlation between serum glucose levels and the severeness of COVID-19 patients.

# Question2 Can you predict COVID deaths by food habits?
We wanted to analyse the data to see if healthy diet plays a factor in low death rate due to COVID-19.
We read the Food_Supply_Quantity_kg_Data.csv using Pandas. This dataset includes percentage of food intake (kg) in countries around the world.
We dropped the columns that we were not interested in. Loaded the John Hopkins confirmed cases and deaths csvs. We merges all the three csvs after clean up.
We also calculated the positive rate and the death rates. 
After analysis we saw that:
Differences in Death Rate can be caused by:
  1. Differences in the number of people tested: With more testing, more people with milder cases are identified. This lowers the Death Rate. 
  2. Demographics: For example, Mortality tends to be higher in older populations.
  3. Characteristics of the healthcare system: For example, Mortality may rise as hospitals become overwhelmed and have fewer resources.
  4. Other factors, many of which remain unknown.
  
 ## Machine Learning
 We ran a Random Forrest regression model and got a score of 0.787.
 Looking at the feature importances, we can see that Animal fats, Sugar and Alcoholic beverges seem to have a high importance in predicting Deaths.
 
 ## Tableau
 Visualizations were created for this dataset. We saw a similar result as above in the process. 
 
 

