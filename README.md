# House-sales-price-prediction

Original dataset has 80 features for house sales price prediction.

Dataset is in file train.

In this repository, we are using 3 techniques for reducing number of features (Random Forest feature selection, Correlation based dimensionality reduction and Autoencoder dimensionality reduction).

1. Feature importance is calculated using Random Forest and then we are keeping first n most important features in dataset.
2. We are reducing features which have correlation with other features greater than threshold. 
3. Autoencoders compress the information of the input variables into a reduced dimensional space and then recreate the input data set.

Instead regression problem, we converted it to classification problem (classes are high, medium and low price) and then comparing accuracy of the Random Forest and Naive Bayes model on reduced features with 3 techniques.
Also we used original values and log transform values. 

The best accuracy for Naive Bayes classification model is with features selected from Random Forest and accuracy is 83%.
The best accuracy for Random Forest classification is with features reduced with correlation and log transform values. Accuracy of this model is 87%.

