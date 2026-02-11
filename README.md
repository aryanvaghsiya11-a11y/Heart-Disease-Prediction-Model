# Heart-Disease-Prediction-Model
🫀 Heart Disease Prediction Model An end-to-end ML pipeline classifying cardiovascular risk with 87% accuracy. Features a robust Scikit-Learn preprocessing architecture and advanced hyperparameter tuning using Optuna. Includes an optimized XGBoost/Random Forest ensemble model ready for clinical deployment. 🚀
This project is a robust machine learning pipeline designed to predict the likelihood of heart disease based on clinical patient data. It encompasses the full data science lifecycle, from comprehensive data preprocessing and exploratory analysis to automated hyperparameter optimization using Optuna and model deployment.

![image alt](https://github.com/aryanvaghsiya11-a11y/Heart-Disease-Prediction-Model/blob/84f64f64b170def029d5a985713e17beccbe0a4a/heart%20disease%20prediction%20model.jpg)

📌 Features
Data Cleaning and Preprocessing

Feature Engineering: Intelligent separation of numerical features (Age, Cholesterol, RestingBP, etc.) and categorical features.

Pipeline Architecture: Implementation of ColumnTransformer for seamless scaling and encoding.

Standardization: Using StandardScaler to normalize numerical distributions.

Encoding: One-Hot Encoding for categorical variables like ChestPainType, RestingECG, and ST_Slope.

Exploratory Data Analysis (EDA)

Distribution Analysis: Visualizing heart disease prevalence across different age groups and genders.

Clinical Insights: Analyzing the correlation between Resting Blood Pressure, Cholesterol, and the target variable.

Correlation Matrix: Identifying the strongest predictors of heart failure.

Automated Hyperparameter Tuning

Optuna Integration: Utilizing Bayesian optimization for advanced tuning of Random Forest and XGBoost.

Trial Management: Executing 100 trials to find the optimal combination of depth, estimators, and learning rates.

Model Training and Evaluation

Classifiers Used:

Logistic Regression (Baseline)

Decision Tree Classifier

Random Forest Classifier

XGBoost (Extreme Gradient Boosting)

Performance Metrics:

Accuracy Score

Precision, Recall, and F1-Score

Confusion Matrix visualizations

Model Persistence

The final optimized pipeline (preprocessing + best model) is saved as final_heart_disease_model.pkl for production readiness.

🚀 Technologies Used
Python 3.x

Pandas & NumPy: Data manipulation and numerical computation.

Matplotlib & Seaborn: Statistical data visualization.

Scikit-Learn: Machine learning algorithms and preprocessing pipelines.

Optuna: State-of-the-art hyperparameter optimization framework.

XGBoost: High-performance gradient boosting library.

Pickle: Model serialization.

📂 Dataset
Input File: heart.csv

Key Features: 11 clinical features (Age, Sex, ChestPainType, RestingBP, Cholesterol, FastingBS, RestingECG, MaxHR, ExerciseAngina, Oldpeak, ST_Slope).

Target: HeartDisease (Binary classification: 1 for disease, 0 for normal).

⚙️ Workflow
Data Loading: Importing the heart disease clinical dataset.

Preprocessing: Building a Pipeline to handle scaling and encoding automatically to prevent data leakage.

EDA: Generating charts to understand the clinical characteristics of patients.

Model Comparison: Training multiple models and evaluating their baseline performance.

Optimization: Running Optuna trials to maximize the accuracy of the Random Forest and XGBoost models.

Final Evaluation: Testing the best-tuned model on unseen data.

Export: Saving the entire pipeline as a .pkl file.

▶️ How to Run
Clone the repository:

Bash
git clone https://github.com/your-username/heart-disease-prediction.git
cd heart-disease-prediction
Install required dependencies:

Bash
pip install pandas numpy matplotlib seaborn scikit-learn optuna xgboost
Data Placement: Ensure heart.csv is in the project root directory.

Execute: Run the heart_disease.ipynb notebook to reproduce the training and optimization process.

📊 Output
Visualization: Feature importance plots and model comparison bar charts.

Metrics: Detailed classification reports for all models.

Saved Artifact: final_heart_disease_model.pkl—a ready-to-use prediction engine.
