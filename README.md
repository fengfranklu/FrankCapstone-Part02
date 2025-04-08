# FrankCapstone-Part02
This is the Part 2 of the Capstone Project for Machine Learning Certificate

## Overview

In this application, you will explore a dataset from Kaggle. The original dataset contained information on over 30,000 movies, spanning 60 years of data. We aim to explore this dataset and determine if a movie rating can be accurately predicted.



## Business Understanding

From a business perspective, if we can predict a movie's rating based on the provided feature values, it will give the movie producer guidance on which movies to produce and which features to prioritize. As such, the company can potentially generate more revenue for each movie they make.



## Notebook

[https://github.com/fengfranklu/FrankCapstone-Part02/blob/main/Frank_Capstone02.ipynb](https://github.com/fengfranklu/FrankCapstone-Part02/blob/main/Frank_Capstone02.ipynb)



## Evaluation and Conclusion

With the inclusion of more numeric fields: meta_score, votes, etc.  the predictive models yield better results than Part1 models. However that budget and gross does not seem to be of importance in predicting the ratings.  The Lasso Regression yield similar results with the Linear Regression model.  The Ridge Regression does not seem to be working correctly, need further investigation if I am using the correct parameters. Just like the part 1 investigation, the Random Forest model still yield the best results and provide the best predictive model.  For further study, I would like to do further statistical analysis to find answers to questions like: Share of total gross earnings by Genre, Top 10 movies with highest ratings, Top 10 movies with highest worldwide gross earnings. etc.  

|      |                Model |   R^2 Score |  Accuracy (%) | Mean Squared Error | Root MSE | Mean Absolute Error |
| ---: | -------------------: | ----------: | ------------: | -----------------: | -------: | ------------------- |
|    0 |    Linear Regression |      0.1951 |  1.951170e+01 |             0.8798 |   0.9380 | 0.6998              |
|    1 |     Lasso Regression |      0.1951 |  1.950550e+01 |             0.8799 |   0.9380 | 0.6997              |
|    2 |     Ridge Regression | -30748.8473 | -3.074885e+06 |         33613.0637 | 183.3387 | 13.0044             |
|    3 | Random Forest (Base) |      0.4781 |  4.780770e+01 |             0.5705 |   0.7553 | 0.5396              |

| Features |        Importance (%) |       |
| -------: | --------------------: | ----- |
|       15 |            meta_score | 15.37 |
|       14 |                 votes | 7.52  |
|        9 |        awards_content | 7.30  |
|       20 |          release_date | 6.56  |
|       10 |                genres | 6.08  |
|       11 |             languages | 6.07  |
|        2 |            Movie_Link | 5.88  |
|        6 |      countries_origin | 5.05  |
|        5 |                 stars | 4.64  |
|        8 |  production_companies | 4.60  |
|        4 |             directors | 4.40  |
|        1 |           description | 4.35  |
|        3 |               writers | 4.25  |
|       12 |                  year | 3.99  |
|        7 |     filming_locations | 3.24  |
|       13 |              duration | 2.48  |
|        0 |                   MPA | 2.07  |
|       18 |       gross_worldwide | 1.81  |
|       16 |                budget | 1.67  |
|       19 |       gross_us_canada | 1.61  |
|       17 | opening_weekend_gross | 1.08  |

![image](https://github.com/user-attachments/assets/9fef8e64-92cc-4564-a727-37a1c29991ea)
