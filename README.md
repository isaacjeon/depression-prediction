# Depression Prediction

This project is in the form of a Jupyter notebook. The dataset can be found here:
https://www.kaggle.com/datasets/sumansharmadataworld/depression-surveydataset-for-analysis/data

The goal of this project is to build a model that predicts whether an individual is at risk of depression based on a number of factors such as age, gender, city, work/study status, etc. It involves performing data cleaning and exploratory data analysis, followed by training and evaluation of models built with several approaches which include Random Forests, gradient boosting with XGBoost, and Support Vector Machines.

The best model used Support Vector Machine (SVM) with a linear kernel, achieving the following results:
- Recall = 98.9%: 98.9% of depressed individuals were correctly identified as depressed (1.1% of actually depressed individuals were incorrectly classified as not depressed)
- Precision = 91.8%: 91.8% of individuals that were classified as depressed were actually depressed (8.2% of non-depressed individuals were incorrectly classified as depressed)
- F1 score = 95.2%: a balanced measure based on recall and precision

This model has particularly high recall, which suggests that it performs well in cases when it is crucial to correctly identify depressed individuals while misclassifying non-depressed individuals as depressed is less of an issue. In fact, misclassifications could actually be meaningful as it could indicate risk of depression in the future.

In addition, from both the correlation matrix from EDA as well as the feature importances from the Random Forests and XGBoost models, I found that age was the most important feature. There was a negative correlation between 'Age' and 'Depression', suggesting that younger surveyees tended to be more likely to be depressed. Other features that were important to a lesser degree involved one's work/study life, followed by features involving lifestyle habits such as sleep and dietary habits.

Through analysis of the results of this project, I was able to identify factors that seemed most correlated with depression along with an classification model that may be effective in detection and prevention of depression.
