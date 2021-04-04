
<h1 align="center">Credit Risk Analysis</h1>

## Overview
The purpose of this analysis is to visualize machine learning techniqe and logistic regression to detect high risk credit profiles.

## Results
The dataset shows an imbalanced split between high risk cases (small portion) and low risk cases (large protion). As such, the analysis has tried 6 different models and below are the results by model.

1. Oversampling Random Over Sampler

In this instance, the high risk cases are over sampled to ensure adequate number of high  risk cases.

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/1_oversampling.PNG)


2. SMOTE

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/2_Smote.PNG)
While the checkout time by gender follows the same pattern as the overall users, it is very clear that males use the bikes more often than the females.

3. Undersampling ClusterCentroids

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/3_Undersampling.PNG)

On weekdays, there are more trips made during rush hours in the morning and in the afternoon. On weekends, there are more trips made during the middle of the day between late morning to early afternoon.

4. SMOTEENN

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/4_overandunder.PNG)

Similar to the pattern we have seen on the checkout times, the trips by gender by hour chart shows that both males and females follow the same pattern by weekday by hour.

5. Random Forest

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/5_randomForest.PNG)

The by user type analysis clearly showed that subscribers use the bikes more often than one off customers.

6. Easy Ensemble

![](https://github.com/lu-chang-axonic/Credit_Risk_Analysis/blob/main/image/6_Easy_Ensemble.PNG)

This chart came from the module. It shows the starting location that has most of the usage. This information can guide the positioning of bikes to ensure ample supply for the demand.

7. Peak Riding Hours

![](https://github.com/lu-chang-axonic/bikesharing/blob/main/Images/Peak%20Riding%20Hours-module.PNG)

This chart came from the module. It shows the usage of bikes by hour. The information can guide the management company in deciding maintenance  time, which seems to be most convenient between 3:00am-4:00am.

## Summary:

In Summary, the analysis shows that the bike sharing project should focus on male subscribers who tend to use the bikes during rush hours on weekdays and off-peak hours during weekends. Most people use the bikes for less than 30 mins. It also shows what locations are most used and provide support on what hours are most suitable for doing maintenance .
Additional two visualizations that I would perform with the given datasets are:

1) Chart the bike usage against birthday year to narrow down to what age group the marketing campain should be target towards.
2) Chart the trip duration against the start time to show what time during the day bikers turn to use bikes for longer/shorter duration.
