What is Cross validation?
The goal of cross-validation is to test the model's ability to predict new data that was not used in estimating it, in order to flag problems like overfitting or selection bias and to give an insight on how the model will generalize to an independent dataset (i.e., an unknown dataset, for instance from a real problem).
Usually the data is split in ratio of 70% for training and 30% for testing.

Types of cross validation:

1. HoldOut Validation Approach- Train And Test Split: plitting the data into multiple parts and using one part for training the model and the rest for validating and testing it. The result cahnges withe change in random state value.

2. K-cross validation: The dataset is divided into k subsets or folds. The model is trained and evaluated k times, using a different fold as the validation set each time. Performance metrics from each fold are averaged to estimate the model's generalization performance

3. Stratified K-fold Cross Validation: is a variation of K-Fold Cross-Validation that ensures each fold maintains the same proportion of observations for each target class as the complete dataset.

4. Repeated Random Test-Train Splits: This technique is a hybrid of traditional train-test splitting and the k-fold cross-validation method. In this technique, we create random splits of the data in the training-test set manner and then repeat the process of splitting and evaluating the algorithm multiple times, just like the cross-validation method.

5. Time series cross validation: This method splits the data into multiple training and testing sets based on a specific time point. For example, the data can be split into training sets from the beginning until a certain date and testing sets from that date onwards.
