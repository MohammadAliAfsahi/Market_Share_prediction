# YapAiTek-assignment
The dataset belongs to the Montreal Local TV channels, which contain some information. The goal is to predict Market Share_total column.

? sklearn

Among different regression algorithm tested, MLPRegressor has the least loss and mean absolute error with high R-squared score.
In order to create a model to predict target column, following steps have take:
1. preprocessing
2. feature engineering
3. choose algorithm and evaluate performance

As For preprocessing data part, First, sklearn LabelEncoder is used, to label each distinct value of a column to a numerical value. Second, Data normalization couldn't help model perfomace for some column.?
Also nan values are treated as follow...

This dataset has 20 columns which one of them is the target column. Among 19 different columns, 13 of have taken as input features for model. These featues are specified in the notebook.

The best result could achieve is for simple multi layered percepton regressor model with following outputs:
- Loss = 3.8081
- mean absolute error = 1.61
- R-squared score = ?
