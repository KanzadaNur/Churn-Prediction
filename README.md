📊 Customer Churn Analysis – Streaming Platform
📌 Project Overview

This project analyzes customer churn behavior for a streaming platform using exploratory data analysis (EDA), statistical testing, and predictive modeling.

The objective is to:

Identify factors influencing churn

Understand behavioral patterns of at-risk users

Provide business recommendations for the retention team

Build predictive models to estimate churn probability

🎯 Business Questions

This analysis answers the following key questions:

Do users who receive promotions churn less?

Does watch time impact churn likelihood?

Are mobile-dominant users more likely to cancel?

What are the top 3 features influencing churn?

Which customer segments should the retention team prioritize?

What factors influence watch time and tenure?

🛠️ Tools & Technologies

Python

Pandas & NumPy

Matplotlib & Seaborn

Scikit-learn

Statistical tests (Chi-square, Welch’s t-test)

Logistic Regression

Linear Regression

📊 Exploratory Data Analysis (EDA)

Key steps:

Churn distribution analysis

Promotion vs churn comparison

Watch time vs churn comparison

Device usage segmentation

Correlation heatmap

Feature engineering:

Tenure (subscription duration)

Watch frequency ratio

Heavy mobile user indicator

🔬 Statistical Testing

To validate hypotheses:

Chi-square test → Relationship between promotions and churn

Welch’s t-test → Difference in watch time between churned and retained users

These tests confirm statistically significant behavioral differences between churned and retained users.

🤖 Predictive Modeling
Logistic Regression (Churn Prediction)

Stratified train-test split

Feature scaling

Class balancing (class_weight='balanced')

Model evaluation

Key findings:

Longer tenure reduces churn probability

Higher watch time reduces churn risk

Mobile-dominant users show higher churn likelihood

Promotions positively impact retention

Top predictive features:

Tenure

Average watch hours

Engagement-related indicators

📈 Linear Regression (Watch Time Drivers)

The model explores factors influencing user engagement (average watch hours).

Insights:

Tenure positively affects watch time

Subscription type influences engagement

Behavioral indicators strongly correlate with watch duration

Note: Engagement is influenced by additional external factors not captured in the dataset.

🧠 Business Insights
🔴 High-Risk Segments

Low-tenure users

Low watch time users

Mobile-heavy users

Users who did not receive promotions

✅ Recommended Retention Strategies

Early lifecycle engagement campaigns

Personalized content recommendations

Targeted promotional offers

Push notifications for mobile users

📌 Key Takeaways

Engagement is the strongest protective factor against churn.

Promotions significantly improve retention.

Behavioral segmentation provides actionable insights for retention teams.

Logistic regression effectively identifies churn drivers.

🚀 Future Improvements

Add ROC-AUC evaluation

Compare models (Random Forest, XGBoost)

Improve feature importance visualization

Add customer lifetime value (CLV) estimation

📂 Repository Structure
├── Week3.ipynb
├── README.md
└── data/
👤 Author

Data analysis project focused on applying statistical reasoning and machine learning to real-world business problems.
