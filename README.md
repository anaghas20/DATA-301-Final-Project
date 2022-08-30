# DATA-301-Final-Project
For the Final Project in Introduction to Data, my group and I focused on how gun legislation correlated with K-12 school shootings and seeing if we could predict the locations of school shootings. Based on the recent school shootings in elementary schools, we wanted to see if gun legislations that were being passed in each state affects the amount of school shootings. We using our skills in data collection, cleaning, visualization, and machine learning to analyze these datasets.

Data Collection and Cleaning: 
-- 
We took in 3 types of data sets: 
  1. Data on K-12 School Shootings 1970-2020 from Center of Homeland Defense and Security
     - An excel workbook with multiple sheets where we used the information about the shooting incidents: location, weapon used, date
  2. Dataset of Gun-Related Legislation Per Year Per State 1991-2017 - A CSV file
     - A CSV file 
  3. Combined One Dataset with Data from US Census API and Population Estimates from 1969-2012
     - Used JSON to access API and Excel file to get a DataFrame of US Population by State 1990-2018
 
Data Exploration 
--
Visualized the trends of K-12 school shootings over time using line graphs and bar graphs. We also looked to compare the rate of school shootings to the states with the highest number of gun legistlations and the states with the least number of gun legislations to find a correlation

Machine Learning
--
We created a machine learning model to predict the location of school shootings based on State, School Level, Time Period, During School, Targets, Situation, Bullied, Preplanned, Weapon Type. We decided to predict the model on the top 3 locations in the database: parking lot, classroom, and beside building, since some locations values rarely appeared in our dataset, and did not provide a solid basis for cross validation. 

Our model, which was decided by having the highest f1 score, the  harmocinc mean of precision and recall, included the variables State, School level, Time Period, During school, Situation, Preplanned, and Weapon type as the predictors.

Test Metrics:
  - This model correctly predicts 71.5% of the locations.
  - Parking Lot: Precision - 79% and Accuracy - 69.5% 
  - Classroom: Precision - 74% and Accuracy - 81% 
  - Beside a Building: Precision - 58.5% and Accuracy - 65.5% 


