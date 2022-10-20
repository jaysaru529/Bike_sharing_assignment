# Bike_sharing_assignment

Observations and explanations from our assignment:

There is an increase in the bike rental count in spring and summer season , and then decrease in the bike rental count in fall in winter season or not.
The bike rental count distribution is higher in 2019 than in 2018.
During no holidays, the bike rental counts is the highest, compared to during holidays for different seasons.
There is no significant change in bike demand with working days and non working days.
During clear, partly cloudy weather, the bike rental count is the highest, second-highest during misty cloudy weather, and followed by 3rd highest, during light snow and light rain weather.
Outlier analysis:
(i) No outliers are present in total_count variable.
(ii) No outliers are present in normalized temp but few outliers are present in normalized windspeed and humidity variables.
Normal probability plot is a graphical technique to identify substantive departures from normality and also it tells about goodness of fit. In our normal probability plot, some target variable data points are deviating from normality.
Correlation matrix tells about linear relationship between attributes and helps us to build better models. From our correlation plot, we can observe that some features are positively correlated and some are negatively correlated to each other. The temp and atemp are highly positively correlated to each other, it means that both are carrying same information.The total_count,casual and registered are highly positively correlated to each other. So, we have ignored atemp,casual and registered variable for further analysis.
For modelling the datset, we split the dataset into train and test in the ratio of 70:30.

Training dataset:
(i) While fitting Linear regression to our trained dataset, Accuracy of the model: 82.4 %
(ii) Cross validation prediction plot tells about finite variance between actual target value and predicted target value. In our Cross validation prediction plot for training dataset, some data points are have same finite variance between them and some are not having it.
(iii) Model Evaluation metrics: R-Squared (R² or the coefficient of determination) is a statistical measure in a regression model that determines the proportion of variance in the dependent variable that can be explained by the independent variable.The R-squared or coefficient of determination for our model is 0.81 on average , it means that predictor is only able to predict 81% of the variance in the target variable which is contributed by independent variables.
Testing dataset:
(i) Model Evaluation metrics: Root Mean Square Error (RMSE) is the standard deviation of the residuals (prediction errors), and The mean absolute error of a model with respect to a test set is the mean of the absolute values of the individual prediction errors on over all instances in the test set.
For our model, Root mean square error : 802.4291866599553 Mean absolute error : 595.2441391283483

Residual plot tells about finite variance between actual target value and predicted target values. In our Residual plot,very less data points are having the same finite variance between them.
