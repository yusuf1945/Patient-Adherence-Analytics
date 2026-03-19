🧠 Predicting Patient Medication Adherence — ML & Power BI Project



This end-to-end healthcare analytics project predicts which patients are at risk of not adhering to their prescribed medication regimen. It integrates machine learning modeling in Python with a multi-tab Power BI dashboard for clinical and operational decision support — ideal for roles like Business Analyst at ProcDNA Analytics.

📂 Dataset Overview
The project uses a synthesized dataset simulating patient adherence behavior, with the following features:



Feature	Description
Age	Patient's age in years
Gender	Binary encoded (0 = Male, 1 = Female)
Dosage_mg	Dosage of medication prescribed (in mg)
Previous_Adherence	Historical adherence indicator (0/1)
Education_Level	Ordinal (None, High School, College, Graduate)
Income	Patient’s annual income
Social_Support_Level	Ordinal (Low, Medium, High)
Condition_Severity	Ordinal (Mild, Moderate, Severe)
Comorbidities_Count	Number of other medical conditions
Healthcare_Access	Ordinal (Poor, Moderate, Good)
Mental_Health_Status	Ordinal (Poor, Fair, Good)
Insurance_Coverage	Binary (0 = No, 1 = Yes)
Medication_Type_*	One-hot encoded columns for TypeA, B, C
Adherence	Binary Target (0 = Non-adherent, 1 = Adherent)



🔧 Project Workflow
1. 🧹 Data Cleaning & Encoding
Handled missing values

Ordinal/binary encoding as per domain schema

One-hot encoding for Medication_Type

2. 📊 Exploratory Data Analysis (EDA)
Correlation heatmaps, distribution plots

Identified key drivers for non-adherence (e.g., Medication_Type, Previous_Adherence, Mental_Health_Status)

3. 🤖 Machine Learning Modeling
Models tested: Logistic Regression, Random Forest, XGBoost

Techniques used:

SMOTE for class imbalance

GridSearchCV for hyperparameter tuning

Best model: Random Forest
ROC AUC: 0.6954
Predictions exported for Power BI integration

4. 💾 Exported Output
Final predictions file: adherence_predictions_for_powerbi.csv

Contains actual + predicted adherence, probabilities, and risk flags



📊 Power BI Dashboard Design
A professional, interactive Power BI report with 4 thematic tabs:


🟦 Tab 1: Overview Dashboard
KPI cards: Adherence rate, High-risk %

Clustered bar: Adherence by Medication Type

Slicers for Gender, Insurance, Risk group


🟩 Tab 2: Patient Analysis
Boxplots for Dosage vs. Adherence

Age and Income distributions

Demographics vs. Risk segmentation


🟥 Tab 3: Risk Analysis
Heatmap: Condition Severity × Social Support

Donut chart: Risk status distribution

High-risk cohort deep dive


🟨 Tab 4: Actionable Insights
Matrix: Suggested interventions (via DAX)

Cards: % without insurance, poor mental health

DAX logic to recommend:

📌 Care coordinator

📌 Community volunteer

📌 Insurance desk referral




🧠 Skills Demonstrated
Data wrangling, feature engineering (Python, Pandas)

ML modeling with scikit-learn, xgboost, imblearn

DAX-based analytics and row-level logic

Storytelling with interactive Power BI dashboards

Business insight generation for healthcare interventions



📁 How to Use
Clone/download the repo

Open and run the Jupyter Notebook for ML pipeline

Open medication_adherence_dashboard.pbix in Power BI Desktop

Use slicers and bookmarks to navigate insights



📈 Potential Use Cases
Pharmaceutical compliance improvement

Hospital patient monitoring

Insurance risk stratification

Targeted intervention planning by NGOs or care coordinators



👨‍💻 Author
Md Yusuful Haque
🎓 B.Tech | 📊 Business Analytics | 💡 Healthcare AI
📧 yusufhaque2020@gmail.com
