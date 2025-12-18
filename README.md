# German Credit Risk Analysis & Prediction

This project focuses on Exploratory Data Analysis (EDA) and Machine Learning to predict credit risk using the German Credit Dataset. The goal is to identify key factors that contribute to "Bad" vs. "Good" credit risk and provide an interpretable model for lending decisions.

## 📊 Project overview
The project follows a full data science pipeline:
- **Data Cleaning:** Handling missing values and translating categorical data.
- **Exploratory Data Analysis (EDA):** Visualizing demographics, loan purposes, and account statuses.
- **Feature Engineering:** Creating new metrics like `amount_per_duration`.
- **Machine Learning:** Training a Random Forest Classifier to predict creditworthiness.
- **Model Explainability:** Using **SHAP** (SHapley Additive exPlanations) to understand the "why" behind the model's predictions.

## 📈 Key Insights from EDA
- **Risk Distribution:** The dataset consists of 70% "Good" and 30% "Bad" credit risks.
- **Loan Duration:** Bad credit risks are significantly associated with longer loan durations (median duration is 5 units higher than good risks).
- **Account Status:** Applicants with no checking account or a zero balance are much more likely to be classified as high-risk.
- **Demographics:** Most applicants are skilled employees who live in rented housing.

## 🔍 Explainability with SHAP
Instead of a "black box" model, this project uses SHAP plots to visualize feature importance:
- **Credit Amount & Duration:** Smaller amounts and shorter durations have a positive impact on credit reliability. As these values increase, the SHAP value turns negative, indicating higher risk.
- **Financial Cushion:** Existing savings and checking account status are among the top decision-making factors for the model.

## 🤓 What I learned
Through this project, I gained practical experience in credit risk analysis:
- **Exploratory Data Analysis (EDA):** I learned how to build a comprehensive profile of credit applicants, identifying patterns in who takes loans, the amounts requested, and the repayment durations.
- **Machine Learning (ML):** I applied ML techniques to reinforce my initial findings and to extract deeper, data-driven insights from the dataset.
- **Model Explainability (SHAP):** I learned how to "open the black box" of machine learning using SHAP. This allowed me to identify the most influential features and understand the specific factors that drive the model's decision-making process.


## 🛠️ Requirements
- Python 3.x
- Pandas
- Seaborn / Matplotlib
- Scikit-learn
- SHAP
