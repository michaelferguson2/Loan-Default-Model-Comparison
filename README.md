# Introduction
The purpose of this project is to find the appropriate binary classification model to determine the likelihood of a potential loan default. As banks take on significant risk in issuing loans, determining the probability of loan default could significantly mitigate risk and help banks and other financial institutions remain profitable.


## Goals 
This project will compare three different classification methods, Logistic Regression, Support Vector Machine, and Random Forest to determine which model may be most successful in correctly identifying potential loan default. To do so, I will analyze and clean the data, set up each model, adjust the hyperparameters, and use the Reciever Operating Characteristic Curve (ROC) and the Area under the ROC Curve (AUC) to determine which model performs best.  

## Data Source
The data for this project comes from [Kaggle](https://www.kaggle.com/datasets/nikhil1e9/loan-default)


# Conclusion
Altogether, the Random Forest Classifier performed much better than the Logistic Regression (Logit) model and slightly better than the Support Vector Machine (SVM) model. With a Balanced Accuracy (BA) score of 0.85 and an AUC score of 0.92, the Random Forest Classifier was better able to correctly identify loan default compared to the Logistic Regression model (BA = 0.75, AUC = 0.86) and the Support Vector Machine model (BA = 0.83, AUC = 0.90). One item to consider is that tree-based methods are more likely to overfit, as such, it may be beneficial to see how well the models perform as the data moves further away from the training data. Given that SVM models can be better generalized, if concerns data are straying far from the training data (for example, a bank opening in a new market with a different customer base) it might be a good idea to implement the SVM model. Otherwise, the Random Forest Classifier model is the preferred choice.
