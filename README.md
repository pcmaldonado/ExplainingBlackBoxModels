# Explaining Black-Box Models
This project is shared on a Medium Article: ["Explaining Black-Box in Python"](https://medium.com/@pcmaldonado/simple-guide-to-interpreting-black-box-models-in-python-5c8bb3b5fcae).

## Overview
When using Machine Learning models to solve real-world problems, it is important to understand how models make their predictions and how features affect them to:
* Make sure that they are not following hidden biases in the data,
* Be able to understand the type of errors the model is making (especially in Computer Vision problems), and to
* Gain a better overall understanding that could help increase business value

The article presents six different model-agnostic techniques that can be used on any Black-Box model.

## Data & Model
To illustrate the different methods, I’ll use a simple Random Forest Classifier to predict High/Low-risk Credit Car Users by using a dataset, from the Public Domain, available on Kaggle. The model is not fine-tuned and obtains a F1-score of 0.71 on the test set.

This type of task requires a good explanation of how the model makes predictions as, if used to accept/decline loans, one needs a good explanation for why applicants may be rejected.

### Tools
This project was done using Python 3.9.7 and the following libraries:
* NumPy, Pandas, Matplotlib, Seaborn, Sklearn, Alibi, Anchor, LIME, SHAP