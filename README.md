Titanic Data Analysis and Machine Learning Model
**Project Overview**
This project focuses on analyzing the Titanic dataset using Exploratory Data Analysis (EDA) and Machine Learning techniques. The dataset is used to predict the survival of passengers aboard the Titanic based on various features like age, sex, passenger class, and more.

**The project involves:**
-Data cleaning and preprocessing.
-Exploratory Data Analysis (EDA) to uncover key patterns and insights.
-Feature engineering to prepare the data for modeling.
-Building a Logistic Regression model to predict survival.
-Evaluating the model's performance.

**Data Source**
The dataset used is from Kaggle's Titanic competition:
 https://www.kaggle.com/competitions/titanic/data

The dataset contains the following columns:
-PassengerId: Unique identifier for each passenger.
-Pclass: Passenger class (1 = 1st class, 2 = 2nd class, 3 = 3rd class).
-Name: Name of the passenger.
-Sex: Gender of the passenger.
-Age: Age of the passenger.
-SibSp: Number of siblings/spouses aboard.
-Parch: Number of parents/children aboard.
-Ticket: Ticket number.
-Fare: Fare paid by the passenger.
-Cabin: Cabin number (with some missing values).
-Embarked: Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton).
-Survived: Target variable indicating whether the passenger survived (1 = Yes, 0 = No).

**Tools Used**
-Python (Pandas, NumPy, Seaborn, Matplotlib)
-Scikit-learn for building and evaluating the Logistic Regression model
-Kaggle for dataset access

**Project Structure**
Titanic-EDA/
│
├── Titanic_EDA_Model.ipynb      # Jupyter notebook with complete EDA and model building
├── Titanic_EDA_Report.pdf       # PDF report summarizing insights and findings
└── README.md                   # Project overview and instructions

**Steps Involved**
1. Data Loading and Overview
The Titanic dataset is loaded using Pandas to get an initial understanding of the data.
Key data characteristics are explored using .info(), .describe(), .value_counts().

2. Data Preprocessing
Missing values in the Age and Embarked columns are filled using median and mode imputation.
The Cabin column is dropped due to a high proportion of missing values.
Categorical variables like Sex are encoded numerically (0 for male, 1 for female).

3. Exploratory Data Analysis (EDA)
Countplots, boxplots, histograms, and scatterplots are used to explore the relationships between different features, especially those that impact survival (e.g., Sex, Pclass, Age, Fare).
Correlation heatmap is used to identify relationships between numerical features.

4. Feature Engineering
New features such as Sex_encoded are created to help with model building.
The dataset is split into features and the target variable (Survived).

5. Model Building
Logistic Regression is chosen as the model for this classification task.
The dataset is split into training and testing sets.
The model is trained on the training data and evaluated using accuracy, precision, recall, and F1-score.

6. Model Evaluation
The Logistic Regression model's performance is evaluated based on its ability to predict survival with accuracy.

**Insights and Findings**
*Key Observations from EDA
-Gender and Survival: Female passengers had a higher survival rate compared to male passengers.
-Passenger Class and Survival: Passengers in 1st class had a higher chance of survival compared to those in 2nd and 3rd class.
-Age and Survival: Younger passengers (especially children) had higher survival rates.
-Fare and Survival: Higher fare-paying passengers were more likely to survive.

*Model Performance
-The Logistic Regression model achieved an accuracy of X% on the test dataset, with precision, recall, and F1-scores indicating good predictive performance.

*Conclusion
The Titanic dataset provides valuable insights into the factors that influenced survival aboard the Titanic. The Logistic Regression model can successfully predict survival, though further feature engineering and model tuning could improve performance.
