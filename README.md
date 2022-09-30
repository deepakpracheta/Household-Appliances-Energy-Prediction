# Appliance Energy Prediction
Today's word usage of energy is increasing rapidly. Due to more usage of energy in some parts of the world, we are facing a lack of energy and it leads to environmental pollution. In some of the places, we are facing outrageous energy consumption in home appliances, so our main goal in this project is to analyse what the factors are affecting the increasing energy consumption of home appliances, how we can reduce the energy consumption of home appliances and predict energy consumption of appliances by using regression models.

## **📖 Abstract:** 
Prediction of the energy consumed by household appliances is a challenging research topic owing to a transition toward the Internet of Everything. In this study, the energy consumptions of appliances were predicted using a ML model based method, wherein the linear, lasso, ridge, decision tree, random forest, gradient boosting, xgb, adaboost and lgbm regression algorithms were employed. The two objectives of the present study were the maximization of the prediction performance of the algorithms and minimization of the number of selected features. The proposed method was tested on the appliances energy prediction dataset which was downloaded from a public dataset from Reliable Prognosis.


## **📖 Dataset information:**
Below are the info that is available in given dataset-
•	lights - Energy use of light fixtures in the house


•	T1 - Temperature in kitchen area 

•	RH_1 -  Humidity in kitchen area. 

•	T2- Temperature in living room area.

•	RH_2 - Humidity in living room area 

•	T3 - Temperature in laundry room area

•	RH_3  - Humidity in laundry room area 

•	T4 - Temperature in office room 

•	RH_4 - Humidity in office room 

•	T5 - Temperature in bathroom 
•	RH_5 - Humidity in bathroom 
•	T6 - Temperature outside the building 
•	RH_6 - Humidity outside the building 
•	T7 - Temperature in ironing room 
•	RH_7 - Humidity in ironing room 
•	T8 - Temperature in teenager room 2 
•	RH_8  - Humidity in teenager room 2 
•	T9 - Temperature in parents room 
•	RH_9 - Humidity in parents room 
•	T_out - Temperature outside (from Chievres weather station )
•	Press_mm_hg - Pressure (from Chievres weather station) 
•	RH_out - Humidity outside (from Chievres weather station) 
•	Windspeed - Wind speed (from Chievres weather station) 
•	Visibility - Visibility (from Chievres weather station) 
•	Tdewpoint - Tdewpoint (from Chievres weather station) 
•	rv1 - Random variable 1 
•	rv2 - Random variable 2
•	Date - Date and time format 
•	Appliances - Energy used by appliances (Target Feature)

## **📖 Problem statement:**
________________________________________
The data set is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network. Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes periods. The energy data was logged every 10 minutes with m-bus energy meters. Weather from the nearest airport weather station (Chievres Airport, Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes (parameters).

## **📖 Approach:**

•	First, we load data set into Panda’s frame and initialize all the library which are required for doing EDA.

•	Then we did inspection of data on a basic level.

•	Then we did data cleaning by removing null values, duplicate values and outliers.

•	Then we used the matplotlib and seaborn to do Exploratory Data Analysis on sample data by plotting different graphs like count plot, pie chart, lmplot, bar plot, boxplot, subplot and heat map from this we got useful insights and correlation between target column and other features

•	In feature selection use variance threshold and F_Regression to select best features

•	In feature engineering check null values, removed outliers in the data set.

•	use multiple models to predict power consumption did hyper parameters tuning Random Forest regression is best model.

•	With model explain ability technique for knowing which features is important

## **📖 Conclusion:**         

•	Many columns in the dataset have not normally distributed and target column is also right skewed
•	Dataset has many outliers and no null values
•	We have hours column is high correlation with dependent variable and there are lot features have lesser than 0.1 correlation with dependent variable and its non-linear dataset.
•	Energy consumption in month of march is high and low in Jan month and increase in temp leads to more energy consumption
•	Decrease in Humidity leads increase in power consumption. Humidity is inversely proportional to dependent variable.
•	Hour of the Day is the most important influencing parameter for Energy consumption
•	High Electricity consumption of >140Wh is observed during evening hours 16:00 to 20:00. Weekends (Saturdays and Sundays) are observed to have high consumption of electricity. (> 25% than Weekdays)
•	Lights are having very low importance as a feature
•	Random forest is the best model its performance is good compare to others have high r2 on test
•	Through model explain ability found which feature has high importance.


## **📖Result**
-  Best model- Random Forest Regressor with 0.70 r2_score.

Here are our **suggestion** :

Upgrading network to improve services for long duration users.
1. Improving Pricing Strategies.
2. Optimizing and Updating International Call Rates.
3. Implmenting a better network infrastructure in New Jersey,Texas and Maryland Areas where there is more Churn Rate.
4. Improvement in the customer service can be done to reduce the number of calls which cause the churn
4. Decreasing the prices as the talk-time increases can be an effective way to reduce the churn.
