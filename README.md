# Predicting median house values in suburbs of Boston in 70s

### **Project Overview**

The purpose of this project is mainly for learning. In this project, the goal was to create a multiple linear regression to predict the median house value in suburbs of Boston in 70s by utilizing a copy of **UCI ML housing dataset** which was taken from [kaggle website](https://www.kaggle.com/datasets/heptapod/uci-ml-datasets). With 3 selected variables, the model had R squared around 0.70 on training data and 0.61 on test data which means at least 61% of the variation of median house value is explained by the model.

### **Business Understanding**

As a real estate company, they want to get the estimate of the property as fast as possible based on some characteristics. When a real estate company know the approximately property's value, they can be more proactive in advertising, dealing, trading and negotiating. It also helps them to avoid mistakes when making business decision, for example pay higher value then the actual value of a property.

### **Data Understanding**

The dataset is a copy of **UCI ML housing dataset** which was retrieved from [kaggle website](https://www.kaggle.com/datasets/heptapod/uci-ml-datasets). The data consisted only 506 observations which was considered small dataset. Beside that limitation, the dataset seems like missing few variations that can affect the median house value. The details of 15 features in dataset are described below:

* CRIM: per capita crime rate by town
* ZN: proportion of residential land zoned for lots over 25,000 sq.ft.
* INDUS: proportion of non-retail business acres per town
* CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
* NOX: nitric oxides concentration (parts per 10 million)
* RM: average number of rooms per dwelling
* AGE: proportion of owner-occupied units built prior to 1940
* DIS: weighted distances to five Boston employment centres
* RAD: index of accessibility to radial highways
* TAX: full-value property-tax rate per $10,000
* PTRATIO: pupil-teacher ratio by town
* B: 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
* LSTAT: % lower status of the population
* MEDV: Median value of owner-occupied homes in $1000's

### **Modeling and Evaluation**

By doing exploratory data analysis, the initial model was built using 3 independent variables: `RM`, `LSTAT` and `CHAS` to predict the target variable `MEDV`. However, the initial model performed not only poor but also violated 2 of 5 assumptions. After re-constructing model by transforming target variable using logarithm, the model proved with better R squared (0.70 for training data and 0.61 for test data).

### **Conclusion**

The model can help a real estate company in 70s gains upperhand when working with property in suburbs of Boston. However, because of small dataset, the model tended to show overfit issues. In order to improve the result, more features should be considered to collected and expanding the number of observations.

<img src=https://i.imgur.com/WfUSSP7.png height=350>


