
<h1 align="center">Credit Risk Analysis</h1>

## Overview
The purpose of this analysis is to visualize machine learning techniqe and logistic regression to detect high risk credit profiles.

## Results
The analysis has tried 6 different models and below are the results by model.

1. Oversampling Random Over Sampler

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/Checkout%20Times%20for%20Users.PNG)

In terms of duration, the vast majority of the users rent the bike for less than one hour, peaking around 10 minuets. This indicates that people are using the bikes to get from point A to point B, rather than for recreation reasons. 

2. SMOTE

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/Checkout%20Times%20by%20Gender.PNG)
While the checkout time by gender follows the same pattern as the overall users, it is very clear that males use the bikes more often than the females.

3. Undersampling ClusterCentroids

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/Trips%20by%20Weekday%20by%20Hour.PNG)

On weekdays, there are more trips made during rush hours in the morning and in the afternoon. On weekends, there are more trips made during the middle of the day between late morning to early afternoon.

4. SMOTEENN

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/Trips%20by%20Gender%20by%20Weekdays%20by%20Hour.PNG)

Similar to the pattern we have seen on the checkout times, the trips by gender by hour chart shows that both males and females follow the same pattern by weekday by hour.

5. Random Forest

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/User%20Trips%20by%20Gender%20by%20Weekday.PNG)

The by user type analysis clearly showed that subscribers use the bikes more often than one off customers.

6. Easy Ensemble

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/Top%20Starting%20Locations-module.PNG)

This chart came from the module. It shows the starting location that has most of the usage. This information can guide the positioning of bikes to ensure ample supply for the demand.

7. Peak Riding Hours

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/Peak%20Riding%20Hours-module.PNG)

This chart came from the module. It shows the usage of bikes by hour. The information can guide the management company in deciding maintenance  time, which seems to be most convenient between 3:00am-4:00am.

## Summary:

In Summary, the analysis shows that the bike sharing project should focus on male subscribers who tend to use the bikes during rush hours on weekdays and off-peak hours during weekends. Most people use the bikes for less than 30 mins. It also shows what locations are most used and provide support on what hours are most suitable for doing maintenance .
Additional two visualizations that I would perform with the given datasets are:

1) Chart the bike usage against birthday year to narrow down to what age group the marketing campain should be target towards.
2) Chart the trip duration against the start time to show what time during the day bikers turn to use bikes for longer/shorter duration.
