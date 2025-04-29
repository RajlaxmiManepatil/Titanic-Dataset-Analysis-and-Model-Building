This project involves analyzing the Titanic dataset and building various machine learning models to predict passenger survival. The steps followed are:

Libraries Used:
pandas for data manipulation.
sklearn for machine learning models and preprocessing.
warnings to suppress warnings.

Data Loading and Initial Analysis
The training and test datasets are loaded from CSV files.
Initial data inspection is performed to understand the structure and identify missing values.

Data Preprocessing
Missing values in the 'Age' column are filled with the mean age, and 'Embarked' missing values are filled with the mode.

New features are created:
Age_cat categorizes passengers as 'child', 'young', or 'old'.
Family_size combines the number of siblings/spouses and parents/children aboard.
iscabin indicates whether a cabin number is provided.
Categorical variables like 'Embarked' and 'Sex' are encoded.
Numerical features 'Fare' and 'Family_size' are scaled using MinMaxScaler.

Model Building and Evaluation
Support Vector Classifier (SVC):

Built and trained with an RBF kernel.
Achieved a training accuracy of approximately 82.8%.
Random Forest Classifier:

Built, trained, and evaluated with default settings.
Achieved a higher training accuracy of approximately 93.7%.
AdaBoost Classifier:

Tuned using GridSearchCV to find the best hyperparameters.
Built and trained with the optimal parameters, achieving an accuracy of 93.7%.
Random Forest Classifier (with GridSearchCV):

Further tuning of hyperparameters using GridSearchCV.
Built and trained with optimized parameters.
K-Nearest Neighbors (KNN):

Built and trained with 9 neighbors.
Predictions were made using the trained model.

