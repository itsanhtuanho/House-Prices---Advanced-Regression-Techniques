# Building a Multiple Linear Regression Model to Predict House Prices

### Introduction  
After taking introductory classes on data science, I decided that my very first data science project should be a multiple linear regression model, a popular technique used to describe a relationship between two or more explanatory
variable and a relevant response variable. One good dataset to engage my machine learning basics was a popular
dataset on house prices, which included data on house prices showcasing 79 potential explanatory variables that can
be used to predict the sale prices of homes.  

One common tip for someone first starting out on their data science journey is prior to starting a project, you should
look at other people's notebooks and notice how others approached the same project for some inspiration. Accordingly,
I looked up the most voted notebook for the dataset on Kaggle and came across Pedro Marcelino's take on the project. 
Within his notebook, he did an extensive detailing on exploratory data analysis. I was thrilled that his focus was on
EDA becuase one of my favorite parts of DS is the visualization aspect and how you can play around with different graphs to gain different insights and explore varying relationships between variables that you want to isolate.  

### About the dataset  
This [dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data) was downloaded from Kaggle. More specifically, I used "train.csv" for this project. It contained 1460 rows with each row representing each home in Ames, Iowa and 79 columns with each column corresponding to a descriptive aspect, such as the year it was built, the square footage of a pool (if there was a pool), and whether or not the driveway is paved.  
### Objectives  
For the sake of simplicity, I will select **6 features** instead of 79 to construct a multiple linear regression model to predict house prices. After completing the model, I will rebuild it and attempt to improve it by **removing outliers**. By eliminating outliers and keeping everything else constant, I can directly understand the impact of having outliers in your model. To evaluate the effectiveness of each model, I will be assessing 3 metrics: **Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and Explained Variance Score**.  
### Metrics  
RMSE and MAE are two popular methods of measuring the average magnitude of the error. MAE measures the average of all absolute errors in a set of predictions wherein the absolute differences between prediction and actual observations have equal weight. On the other hand, RMSE calculates the square root of the average of squared differences between prediction and actual observations. In other words, RMSE is the square root of the variance of residuals. With regards to RMSE and MAE, lower values are preferred and indicate better fit. Explained variance measures the model's total variance that can be explained by factors that are actually included in the model and isn't due to error variance.
