#🛣️ Intelligent Classification of Rural Infrastructure Projects

📜 Project Overview
This project automates the classification of Pradhan Mantri Gram Sadak Yojana (PMGSY) rural infrastructure projects into their respective schemes (PMGSY-I, PMGSY-II, RCPLWEA, etc.) using Machine Learning.

The PMGSY program provides all-weather road connectivity to unconnected rural habitations across India.
Manual categorization of thousands of road and bridge projects is time-consuming, error-prone, and inefficient.

We developed a multi-class classification ML model that predicts the correct PMGSY scheme based on the physical and financial characteristics of each project.

🎯 Objectives

Automate classification of road/bridge projects into correct PMGSY scheme.

Improve monitoring, budgeting, and transparency in rural development.

Minimize manual errors and reduce time spent in project verification.

Deploy the model on IBM Cloud Lite services for scalability.

🗂️ Dataset

Source: AI Kosh – PMGSY dataset

Records: ~20,000+ project entries (varies by version)

Features:

Categorical: STATE_NAME, DISTRICT_NAME

Numerical: project counts, road length, bridges, sanctioned costs, expenditures, balances

Derived features: COST_PER_KM, EXPENDITURE_RATIO, COMPLETION_RATE_ROAD

Target: PMGSY_SCHEME (multi-class label)

🧰 Technologies Used

Programming Language: Python

Libraries: Pandas, NumPy, Scikit-learn, Joblib, Matplotlib

Models: Random Forest Classifier, Logistic Regression, AutoAI (optional)

Environment: Jupyter Notebook, IBM Watson Studio

IBM Cloud Services:

IBM Cloud Object Storage

IBM Watson Studio

IBM Watson Machine Learning

IBM AutoAI (optional)

⚙️ Model Performance

Metric	Score (baseline RF)
Accuracy	~95% (varies by fold)
Precision	~94%
Recall	~94%
F1-Score	~94%

Strong classification performance across PMGSY scheme categories.

Key predictive features: sanctioned cost, road length, expenditure ratio, completion rate.

📊 Visualizations

Confusion Matrix for classification results

Feature Importance ranking (e.g., COST_PER_KM, EXPENDITURE_RATIO)

Distribution of projects by scheme and state
