# Liver-cirrhosis-prediction
### In this Project we will try to Predict liver Cirrhosis disease. Cirrhosis is a late stage of Scarring (fibrosis) of the liver caused by many forms of liver diseases and conditions, such as hepatitis and chronic alcoholism.


## About
Liver cirrhosis is a widespread problem especially in North America due to high intake of alcohol. In this project, we will predict liver cirrhosis in a patient based on certain lifestyle and health conditions of a patient.

## Data set: 
This data set is available on [Kaggle](https://www.kaggle.com/datasets/fedesoriano/cirrhosis-prediction-dataset/code?resource=download) which was collected from the Mayo Clinic trial.

This data set has about 20 features. These features are related to the patient’s details like age, sex, etc. and patient’s blood tests like prothrombin, triglycerides, platelets levels, etc. All these factors help in understanding a patient’s chances of liver Cirrhosis.

Again, the challenges for this dataset are the null values which need to either be replaced or deleted. Also, this data set has unbalanced classes, so it might require up-sampling the dataset.

### Algorithm:

We can use the Random Forest Classifier for this as well as the XGBoost Classifier for this model. A good practice is to train the data on both of these models and choose the model with the best scores. From xgboost, we can import XGBClassifier.

### Implementation:

First, perform some data cleaning, check the outliers and null values. Outliers can be checked by calculating the z-score of the dataset and keeping a threshold value beyond which the data values will be considered outliers. Then do some Exploratory data analysis and visualizations to understand the data better. When splitting the data into training and test sets, use Stratified K-fold to ensure the target variable is equally balanced in all the test and training splits. It can be done by importing StratifiedKFold from sklearn.model_selection. Then train the data on both the models and choose the model based on the performance metrics like precision, recall, accuracy, etc. From sklearn.metrics, you can import classification_report, accuracy_score, precision_score, recall_score to check the performance metrics.


