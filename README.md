# Estimation of Obesity Levels Based on Eating Habits and Physical Condition

Data source : [UCI Dataset](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition)  
Data's introductory paper : [View on Semantic Scholar](https://www.semanticscholar.org/paper/Dataset-for-estimation-of-obesity-levels-based-on-Palechor-Manotas/35b40bacd2ffa9370885b7a3004d88995fd1d011)

The dataset utilized in this study is sourced from the UCI Machine Learning Repository and comprises 2111 records with 17 attributes. According to the introductory paper, the data was initially collected through a webpage survey designed to assess participants’ eating habits and various physical condition attributes. The original data exhibited class imbalance, prompting the use of the Weka tool and the SMOTE filter to generate synthetic data. Approximately 77% of the data is synthetic, while the remaining 23% consists of the original data. Since this is a augmented dataset, it does not have any missing values.

Upon detailed examination of the dataset, it was observed that the data generated using the Weka tool and the SMOTE filter was incorrectly processed. Specifically, categorical variables were treated as continuous, resulting in values being represented in decimals, which is inappropriate for such data types. After removing all rows containing the inaccurately processed data, we were left with 513 rows of correct data.

In the remaining data, a noticeable imbalance was observed in the Obesity Levels. To mitigate this issue and ensure a balanced representation of Obesity Levels, we intend to generate synthetic data. To achieve this, we will utilize SMOTE-NC, an extension of the Synthetic Minority Oversampling Technique (SMOTE) designed to handle both numeric and categorical data.
