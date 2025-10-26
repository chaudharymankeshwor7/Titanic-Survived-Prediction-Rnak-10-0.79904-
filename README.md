🧭 Repository Title

Titanic Survival Prediction – Advanced Feature Engineering & Ensemble Modeling

📝 Project Description

This project focuses on predicting passenger survival on the Titanic using advanced feature engineering, exploratory data processing, and ensemble learning techniques. The dataset is taken from the well-known Kaggle Titanic: Machine Learning from Disaster competition.

Key highlights of this project include:

Comprehensive data preprocessing with intelligent handling of missing values.

Feature extraction from complex fields such as Name, Ticket, and Cabin.

Creation of new informative features like:

Family_Size, Is_Alone, Deck, Title

Group-based survival rates: Family_Survival_Rate, Ticket_Survival_Rate

Interaction features like Sex_Pclass, Age_Pclass, and binned variables (AgeBin, FareBin).

Encoding of categorical variables using LabelEncoder, OneHotEncoder, and OrdinalEncoder.

Model training using RandomForestClassifier and GradientBoostingClassifier, with Stratified K-Fold Cross-Validation for robust evaluation.

Both models were compared based on AUC and Accuracy, and the Random Forest model performed better overall.

⚙️ Tech Stack

Language: Python

Libraries: NumPy, Pandas, Scikit-learn, XGBoost

Environment: Jupyter Notebook / Python Script

📊 Model Performance
Model	Avg CV AUC	Avg Accuracy	Final Public Score
Random Forest	~0.84	~0.81	0.79904
Gradient Boosting	~0.83	~0.80	—

✅ Final submission was made using Random Forest, achieving a Kaggle Public Score of 0.79904.

🚀 How It Works

Load and merge training and test data.

Handle missing values using median, mode, and grouped transformations.

Feature engineering:

Extract decks, ticket prefixes, family information, and name titles.

Create binned variables (AgeBin, FareBin) and derived ratios.

Add survival rate features for families and tickets.

Encoding categorical data using a mix of label, one-hot, and ordinal encoders.

Feature selection using Recursive Feature Elimination (RFE) with a RandomForestRegressor.

Model training & evaluation with 5-fold Stratified Cross-Validation.

Generate predictions for test data and export final submission as submission_0.csv.

🧩 Files

train.csv – Training dataset

test.csv – Test dataset

titanic_model.py – Complete training and prediction script

submission_0.csv – Final submission file (Random Forest output)
