# Appliances-Energy-Prediction
Data-driven prediction of energy use of appliances

In this time of global uncertainty world needs energy and in increasing quantities to support
economic and social progress and build a better quality of life, in particular in developing
countries. But even in today’s time there are many places especially in developing world where
there are outages. These outages are primary because of excess load consumed by appliances at
home. Heating and cooling appliances takes most power in house. In this project we will be
analysing the appliance usage in the house gathered via home sensors. All readings are taken at
10 mins intervals for 4.5 months . The goal is to predict energy consumption by appliances . In the age of smart homes, ability to predict energy consumption can not only save money for end
user but can also help in generating money for user by giving excess energy back to Grid (in case
of solar panels usage). In this case regression analysis will be used to predict Appliance energy
usage based on data collected from various sensors. The dataset consists of 29 columns and we
additionally created 9 more column. As the first step we perform data wrangling over the raw data. Further. we divided the complete
project into 5 main parts ie Data Processing I, Data Processing II, EDA, Applying Models and
then Model Validation and Selection. In Data Processing I, we focused mainly on the features of the data and we learnt about columns
and removed unnecessary features and found missing values if any. For Data Processing II, we manually go through each features and define dependent and
independent variables selected from part 1, encode the categorical features and also defining the
target variable(Appliances). Next, we do some exploratory data analysis (EDA) on the features selected in part-1 and 2 and
also visualize the data to see the trend and understand more about the features. Through
visualization techniques such as boxplot, bar graphs and line plots and other, we have identified
the time of day when energy consumption is more as compared throught the day. Finally, In this last but not the last part, we create models. It's an iterative process. We should
predict Appliance energy consumption for a house based on factors like temperature, humidity &
pressure . In order to achieve this, we need to develop a supervised learning model using
regression algorithms. Regression algorithms are used as data consist of continuous features and
there are no identification of appliances in dataset. Extra Trees Regressor performed the best with
default parameters. Feature scaling is very important for regressions models. Hyper parameter tuning for the best algorithm and reporting the test score of best model. I used
grid search cross validation using the GridSearchCV function of the sklearn.model_selection
library. The R2 score improved by 1% (0.58 to 0.59) post usage parameters suggested by
GridSearchCV. On reduced features dataset the GridSearch CV was able to show upto 63%
accuracy. The top 3 important features are humidity attributes, which leads to the conclusion that humidity
affects power consumption more than temperature. Windspeed is least important as the speed of
wind doesn’t affect power consumption inside the house. So controlling humidity inside the house
may lead to energy savings.
