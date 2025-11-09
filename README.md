📡 Telecom Customer Churn Prediction
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/166e0daa-ecf1-4389-bbd2-d04725ffcf50" />


An end-to-end machine learning project to predict customer churn in telecom using XGBoost, deployed with Streamlit.

🏷️ Badges
<p> <img src="https://img.shields.io/badge/Python-3.10-blue"/> <img src="https://img.shields.io/badge/ML-XGBoost-yellow"/> <img src="https://img.shields.io/badge/Framework-Streamlit-red"/> <img src="https://img.shields.io/badge/Deployment-Cloud-green"/> <img src="https://img.shields.io/github/stars/yourrepo?style=social"/> </p>
🎥 Demo
<p align="center"> <img src="/images/app_demo.gif" width="800"/> </p>

🔗 Live Application:

(https://churn-prediction-data.streamlit.app/)

✅ Table of Contents

Overview

Business Objective

Dataset

Workflow

EDA Highlights

Modeling

Confusion Matrix & Explanation

Conclusion

Tech Stack

Project Structure

Deployment

Run Locally

Documentation

Future Enhancements

Author

🚀 Overview

Customer churn is a major financial risk for telecom companies.
Using historical customer usage & service data, this ML system predicts whether a customer is likely to churn.

✅ Feature engineering
✅ EDA
✅ XGBoost modeling
✅ Streamlit UI
✅ Deployment

🎯 Business Objective

Telecom companies lose millions to churn every year.
This project aims to:

✔ Identify churn-prone customers
✔ Understand churn drivers
✔ Enable retention strategies
✔ Improve revenue stability

📦 Dataset

Each row represents one customer.

Feature	Description
account.length	Duration active
intl.plan	Yes/No
voice.plan	Yes/No
day.mins	Minutes/day
night.mins	Minutes/night
customer.calls	Complaint calls
churn	Target (Yes/No)

Total Customers → 667

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/decaafe0-9554-44e5-ac2c-9b95aff52385" />


1️⃣ Data Loading
2️⃣ Cleaning & Preprocessing
3️⃣ EDA
4️⃣ Feature Selection
5️⃣ Model Training (XGBoost)
6️⃣ Evaluation
7️⃣ Streamlit App
8️⃣ Deployment

🔎 EDA Highlights

✅ Customers with international plan churn more
✅ Higher customer service calls → churn
✅ Usage patterns differ between churn & non-churn

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/58319ee7-229c-4e32-a5a4-939a666e95f1" />

🤖 Modeling

We trained multiple models:

Model	Accuracy
Logistic Regression	~90%
Random Forest	~97%
XGBoost	✅ 98% (Best)

Final model → XGBoost
Reason → Highest accuracy + strong generalization

✅Classification Report
              precision    recall  f1-score   support

           0       0.98      1.00      0.99       566
           1       1.00      0.87      0.93       101

    accuracy                           0.98       667
   macro avg       0.99      0.94      0.96       667
weighted avg       0.98      0.98      0.98       667

🔍 Interpretation:

✅ Class 0 perfectly recalled (1.00)
✅ Class 1 is well captured (recall 0.87)
✅ Very high precision for both classes
✅ Overall model is highly reliable

✅ Conclusion

✔ XGBoost model achieved 98% accuracy
✔ Excellent ability to detect non-churn customers
✔ Strong performance on churn prediction

🔹 Key churn indicators:

International plan = higher churn

High customer service calls

Usage patterns

✅ Business Value:
Allows targeted retention → reduced churn → increased revenue

Inference:

Out of 667 customers →

566 were predicted correctly as non-churn

101 were predicted correctly as churn

Extremely low misclassification

XGBoost outperformed Random Forest (97%)

✅ Conclusion

✔ Built an end-to-end customer churn prediction system
✔ XGBoost provided highest accuracy → 98%
✔ Very high capability in capturing churn behavior
✔ Key churn indicators:

🔹 International Plan
🔹 High Customer Care Calls
🔹 Daily usage patterns

Business Impact:
Early flagging enables retention teams to contact high-risk customers →
✅ Lower churn
✅ Higher revenue
✅ Increased customer lifetime value

⚙ Tech Stack
Category	Tools
Language	Python
ML	XGBoost, Scikit-Learn
Data	Pandas, NumPy
Viz	Matplotlib, Seaborn
Deployment	Streamlit
Version Control	Git + GitHub
📁 Project Structure
📦 Telecom-Churn-Prediction
│
├── data/
├── notebooks/
│   └── TELE_COMMUNICATION.ipynb
├── models/
│   └── xgboost_model.pkl
├── app/
│   └── app.py
├── images/
│   └── banner.png
│   └── app_demo.gif
│   └── logos...
├── docs/
├── requirements.txt
├── README.md
└── LICENSE

🌐 Deployment

✅ Deployed using Streamlit Cloud

🔗 Live App →

(https://churn-prediction-data.streamlit.app/)

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/ad7d0800-9c3d-47c6-b603-0e0f9dab7efe" />

🏃 Run Locally
# Clone repo
git clone(https://github.com/shashankphenomeno111/Data-science-Project-TELE-COMMUNICATION-.git)
cd YOUR_REPO

# Install deps
pip install -r requirements.txt

# Run app
streamlit run app.py

📘 Documentation

📂 In /docs/
✔ EDA summary
✔ Business requirements
✔ Model evaluation

🔮 Future Enhancements

✅ API integration
✅ Real-time churn scoring
✅ Customer segmentation
✅ Auto model retraining
✅ CRM integration

👤 Author

Shashank R

📧 Email :shashankphenomenon@gmail.com
🔗 LinkedIn :


