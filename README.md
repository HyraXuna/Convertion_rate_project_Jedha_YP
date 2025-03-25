# Convertion rate project

[![forthebadge](http://forthebadge.com/images/badges/built-with-love.svg)](http://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)

This is the 2nd supervised machine learning project. The goal is to test different models and to find one with the best f1-score of a model that predicts if a given user will subscribe to the newsletter, by using just a few information about the user.

## Getting Started

All the models tested are in this [Notebook](Conversion_rate_challenge_YP.ipynb).
* EDA
* Preprocessing
* Baseline model
* Feature engineering
* Other model test & train
* Conclusion

All of that with confusion matrix & f1-score evaluation 📈.

### Prerequisites

Things you need to run the codes:

```
python 3.12.1

pandas 
numpy
scikit-learn
matplotlib
plotly
plotly.express
plotly.graph_objects
```

### Some Results

Here some example of f1-score results for some tested model:

* Basic Logistic Regression after feature engineering:
```python
f1-score on train set :  0.7633393586396198
f1-score on test set :  0.7719087635054022
````
![image](https://github.com/user-attachments/assets/13b77227-885a-4440-98d3-654f8f3f2404)
![image](https://github.com/user-attachments/assets/5ef64f75-8264-40cf-960e-b8f5db577ad5)

* XGBoost:
```python
f1-score on train set :  0.7675962815405046
f1-score on test set :  0.7701421800947867
```

* MLPClassifier:
```python
f1-score on train set :  0.7652382219856269
f1-score on test set :  0.7692307692307693
```

We can't reach an higher score at one moment due to the qualitate of the dataset to studied. We have a lot of 0 and less 1 so the different models are limited to learn for the prediction of 1. That means we are obligated to have a partial error on it that stop the maximum f1 score around 0.75, 0.76. But with the testing data of Jedha, my best model is the Gradient boosting classifier.

## Acknowledgments

* Thanks for Jedha and its instructors for the lectures, exercises and all the work.

