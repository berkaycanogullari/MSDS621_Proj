[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/berkaycanogullari/MSDS621_Proj/blob/main/project_notebook.ipynb)

# Can online customers' intention be predicted beforehand?
---

## Who am I?

My name is Berkay Canogullari. I'm currently pursuing my M.S. in Data Science at the University of San Francisco. At the same time, I'm working as a Machine Learning Researcher at the University of California, San Francisco!

---

## About the project

In this project I'm going to try to predict if a customer causes revenue to the company based on the features of the [dataset](https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset#) and compare two fundamental ML algorithms. My main focus will be to show Scikit-Learn's general functionality and predictive power but **not** interpretability. I will explain what steps I took and why over the project notebook.

---

## Why is it important?

Customers who aren’t making a purchase can be analyzed in detail and further action can be taken accordingly to increase revenue

---

## Findings

1) Random Forest algorithm performed better than logistic regression in terms of predictive power
2) Time to do hyperparameter search with cross validation for Random Forest was relatively longer than the Logistic Regression model
3) Based on balanced accuracy and recall, our model performs relatively well. 84.2% and 79.6% respectively
4) By looking at precision score(56.7%), we can see that our model is over-predicting a user causing a revenue and performing poorly in that sense. This might be a result of having an imbalanced dataset
5) f1 score of 66.2% suggests that the model performs okay if we care equally about recall and precision
6) **Overall**: Our model's performance depend on what we expect from it and the business goals. It doesn't perform great in every aspect, but it performs well in terms of accuracy and recall.

---

## Next Steps

1) Features that are found to be bad by permutation importance can be taken out from the model and retraining can be done to see if there will be an improvement
2) More data can be collected for the minority class, if it makes sense in terms of cost/return
3) Different prediction algorithms can be added for better performance comparison, ex. LightGBM
