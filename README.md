# loan_prediction_model

* Steps for pre-processing
    * Imported the csv and converted it into dataframe
    * Categorized the the train and test dataset into features and target for analysis
    * Transformed Categorical target values to numerical using sklearn's LabelEncoder
    * Converted Categorical features values to indicator variables using the pandas.get dummies 
    * The test dataset was missing a column as one of the categorical variables in the test dataset was        identical throughout the dataset and the train dataset had a binary set of values. Added the missing column with 0 as values. 

* Working with Unscaled Data    
    * Use Logistic Regression Model from sklearn's linear_model module to train and fit the unscaled data to check the accuracy score on the test data.
    * Use Random Forest Classifier Model from sklearn's ensemble module to train and fit the unscaled data to check the accuracy score on the test data.

* Scaling the Data 
    * Scale the data using Standard Scaler from the sklearn's preprocessing module

* Working with Scaled Data
    * Use Logistic Regression Model from sklearn's linear_model module to train and fit the scaled data to check the accuracy score on the test data.
    * Use Random Forest Classifier Model from sklearn's ensemble module to train and fit the scaled data to check the accuracy score on the test data. 

* Conclusions
    Random Forest Classifier Model works better with unscaled data than Logistic Regression Model. This is confirmed by the analysis and completely understandable as the data has not been optimized to use the Logistic Regression Model. Once the data is scaled Logistic Regression Model is a much better predictor of the risk of a particular loan as the data is now optimized as Logistic Regression is a much better model to generate a binary result. 