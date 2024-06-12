INTRODUCTION:
The purpose of this report is to present the results and main strategies of DATA MINING project using ecg_signal Dataset. The goal of the project was to achieve a high accuracy and classifying into different categories. Data Mining techniques help extract meaningful insights from large volumes of data.

DATASET OVERVIEW:
This dataset containing 31 features was obtained by processing the provided ECG signals all are numerical, and the target variable is also encoded. we load the dataset which was in CSV format with Pandas dataframe.


IMPORTING LIBRARIES:
To accomplish the DATA MINING task on the ECG_SIGNAL Dataset, several libraries were utilized. These libraries provided essential functionalities for data handling, model creation, training, and evaluation. The following libraries were imported:

PRE-PROCESSING:
After loading the dataset, we have created the data to new dataframe. Using basics of pandas, we displayed pandas properties like ( info(), shape, describe(), isnull() etc) and we converted all columns of the dataset to float.


CORRELATION:
   
We have separated the dataframe with all the columns into X variables and the column ‘label’ to another variable Y which is last column of the dataframe and it also contains the target variable of the output variable of the dataset. Typically, this kind of split is done to separate the input variable from the output variable so that we can use input variables to predict the output variable. We used the Heatmap to check the correlation between features.

FEATURE SELECTION AND EXTRACTION:
For Feature selection, we have used multiple feature selection techniques such as SelectKbest, SelectFromModel, Sequential Feature selector and also SelectFromModel embedded method to find the most important features that are more important to the target variable. The features that were more common in all the 5 feature selection models done have been selected.




TRAINING AND TESTING THE MODEL:
The data is then split into Train and Test data with 70% and 30% respectively using Traintestsplit with Scikit learn. Various Machine Learning models are used to check which model has the best performance. The classification models used for detecting the emotions are: Logistic Regression,KNeighboursClassifier,SVM Classifier and DecisionTreeClassifier.
We compared the each models, we got accuray for each model. Logistic Regression is 75%, KNeighbour Classifier is 81%, SVM Classifier is 79%, and Decision Tree Classifier is 69%.
CONFUSION MATRIX:
We also obtained, the selected models are evaluated using Confusion matrix to check whether precision and recall are balanced. The f1 score is used to evaluate the precision and recall balance.



CONCLUSION:
In conclusion, the results of this experiment provide valuable insight into the performance of different machine learning models for binary classification problems. Model SVM Classifier was found to be the most accurate and can be considered for further analysis and implementation in the future. We had build the same models using PCA dataset and compared the accuracies provided by the algorithm.The steps involved in the project, including data pre- processing , feature selection, data split, model building and training, model comparison, and unsupervised learning were described in detail.
