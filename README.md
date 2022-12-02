
#  Predicting the processing duration of a model, Using ML
The Dataset given to us included features such as  type, time, day of week, models, parameters, queue length and trials.

This was a competition for shortlisting ML interns for the startup Chi SquareX

1st May 2022 to 6th May 2022


## 🔗 Links
[kaggle competion link here](https://www.kaggle.com/competitions/chisquarexhiring)

Username : Noob:)

## Tools and Techniques Used
- Data Exploration using Seaborn(heatmap, kde plots)
- Removing outliers using boxplot(Seaborn) 
- Collected categories whose mean of duration was in a range close to target values and best range was chosen for all the features
- Encoded them with their respective updated target values and filled nan values with 0
- Target Values were updated as [0:10,1:20,2:30,3:40] so that our model can distinguish 0(nan) from our target values 
- As time was a continuous feature therefore ranges of time period were encoded
- test and train dataset had similar outliers with respect to params and queue_len and hence only outliers of 'models' column were removed 
- various methods such as random_imputation /mean /median /mode /prediction by model training were tried to fill nan values of type and params columns, out of which random_imputation was chosen for both of the features
- Since the dataset was imbalanced with respect to target feature hence ensembling models were tried like Random Forest with Scikit-Learn, XGBoost, LightGBM, and CatBoost,and Catboost was chosen as the final model,based on cross validation score

### Ranked 21st among 90 teams
