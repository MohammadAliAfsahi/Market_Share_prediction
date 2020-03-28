# YapAiTek-assignment
The dataset belongs to the Montreal Local TV channels, which contain some information. The goal is to predict Market Share_total column.

Required libraries are pandas, numpy, sklearn and keras, but most of the notebook is written with sklearn, pandas and numpy.

Among different regression algorithm tested, MLPRegressor has the least loss and mean absolute error with high R-squared score.
In order to create a model to predict target column, following steps have take:
1. preprocessing
2. feature engineering
3. choose algorithm and evaluate performance

As For preprocessing data part, First, sklearn LabelEncoder is used, to label each distinct value of a column to a numerical value. Second, Data normalization is just done on 'Temperature in Montreal during episode' column with range between -1 and 1.

Among chosen features, 'Temperature in Montreal during episode', 'Start_time and 'End_time' has nan values. In 'Temperature in Montreal during episode' column nan values are replaced with mean. But in other two, 'Start_time' and 'End_time', first they've got converted to categorical like morning, noon, evening and so on. Then using sklearn LabelEncoder, each got distinct label.

This dataset has 20 columns which one of them is the target column. Among 19 different columns, 13 of have taken as input features for model. These featues are specified in the notebook.

The best result could achieve is for simple multi layered percepton regressor model with following outputs:
- Loss = 1.943
- mean absolute error = 1.25
- R-squared score = 0.83
