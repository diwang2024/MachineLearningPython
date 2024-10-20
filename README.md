# MachineLearningPython
Project for the online course [Machine Learning with Python](https://jovian.com/learn/machine-learning-with-python-zero-to-gbms) at [Jovian](https://jovian.com). It can be run on Google Colab or Kaggle. In this project, I use a [Kaggle dataset](https://www.kaggle.com/c/instacart-market-basket-analysis/data) of Instacart Market Basket Analysis to predict consumers' repurchase decision of bananas based on the product characteristics and consumers' previous purchase behavior. I mainly use the various functions of `sklearn` package.

In this project, I do the following.
- Download and clean the dataset. Take a small slice (5%) of the data (around 70,000 rows).
- Perform exploratory data analysis to examine relevant patterns of repurchase
- Prepare the dataset for ML training: split the train/validation set, impute missing values, scaling, encoding, etc.
- Train a logistic regression model, achieving an accuracy score for the validation set of 60.41%
- Perform feature engineering
- Train a gradient boost model with K-fold cross validation
- Tune hyperparameters to achieve RMSE error of 1/4 of an SD

Here are some relavant features that help with the prediction.
- The number of times that the product was bought in the three most recent orders
- Whether the product was repurchased in the most recent order
- The number of orders that the user has placed before
- The number of days that the user has recently gone without the product
