# Predicting the Severity of Car Accidents
In this project, I build a machine learning model to predict the severity of car accidents based on different attributes such as weather conditions, road conditions, time of day, and location. By predicting the severity of an accident, we can help emergency responders allocate resources more efficiently and potentially save lives.

# Analyzing US Accidents Dataset
The dataset used in this analysis is the "US Accidents" dataset, which can be found on Kaggle here https://www.kaggle.com/sobhanmoosavi/us-accidents. This dataset contains information on traffic accidents that occurred in the United States from February 2016 to December 2019. It includes over 49 million records, making it one of the largest publicly available datasets on traffic accidents.

# Data Cleaning and Preprocessing
The notebook begins with data cleaning and preprocessing steps. The first step is to remove any columns that are not relevant to the analysis, such as 'TMC', 'End_Time', and 'Description'. Next, the missing values are checked for each column and are either removed or imputed with appropriate values. The data types are then adjusted as needed, for example, changing 'Start_Time' and 'End_Time' columns to datetime format.

After preprocessing, the dataset contains information on accidents such as location, severity, time, and weather conditions. These variables are explored through various visualizations, including maps, histograms, and bar charts. Some of the key insights from the exploratory analysis include:

California has the highest number of accidents, followed by Texas and Florida.
Accidents are most common during rush hour periods and on weekdays.
Most accidents are minor, with only a small percentage being fatal or causing severe injuries.
Weather conditions such as clear and cloudy are the most common during accidents.
Feature Engineering
The next step is to engineer additional features that may be useful for modeling. The 'Start_Time' column is used to create new columns for the day of the week, hour of the day, and month of the year. The 'Weather_Condition' column is also used to create a binary column indicating whether the weather was bad or not.

# Model Training and Evaluation
The final step is to train machine learning models to predict accident severity based on the available variables. Three models are trained and evaluated: logistic regression, random forest, and XGBoost. The dataset is split into training and testing sets, and the models are trained on the training set and evaluated on the testing set using various metrics such as accuracy, precision, recall, and F1 score.

The XGBoost model performs the best, achieving an accuracy of 73% and an F1 score of 0.63. The feature importance of the XGBoost model is also analyzed to identify the most important variables in predicting accident severity.

# Conclusion
In conclusion, this notebook presents an analysis of the US Accidents dataset, exploring the variables that contribute to accident severity and training machine learning models to predict accident severity. The results of the analysis can be used to inform policy decisions and improve road safety measures.

