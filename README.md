📊 Customer Churn Analysis – Streaming Platform
📌 Project Overview

Customer churn prediction is an important problem for subscription-based businesses such as streaming platforms. Retaining existing users is significantly more cost-effective than acquiring new customers.

This project analyzes user behavior to identify factors that influence churn and builds predictive models to estimate churn probability.

The analysis combines exploratory data analysis (EDA), statistical testing, and machine learning models to generate actionable business insights.

🎯 Business Questions

This analysis aims to answer the following key questions:

Do users who receive promotions churn less?

Does watch time impact churn likelihood?

Are mobile-dominant users more likely to cancel?

What are the top features influencing churn?

Which customer segments should the retention team prioritize?

What factors influence watch time and user tenure?

🛠 Tools & Technologies

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

📊 Exploratory Data Analysis
Churn Distribution

Insight

This chart shows the distribution of churned versus retained users in the dataset.
![Churn Distribution](https://raw.githubusercontent.com/KanzadaNur/Churn-Prediction/main/images/distrubition_churn.png)
Key observations:

The dataset contains both churned and retained users.

Churn represents the minority class, which is typical in subscription businesses.

This class imbalance must be considered when building predictive models.

To address this issue, the logistic regression model uses class balancing to ensure churn cases are properly identified.

📊 Promotions vs Churn

Insight

This visualization compares churn rates between users who received promotional offers and those who did not.
![Promotion vs Churn](https://raw.githubusercontent.com/KanzadaNur/Churn-Prediction/main/images/distr_rec_promotion_churn.png)
Key findings:

Users who receive promotions show lower churn rates.

Promotional incentives appear to improve customer retention.

Promotions may help maintain engagement with the platform.

Business Implication

Retention teams should consider targeted promotional campaigns for users showing early signs of churn risk.

📊 Watch Time vs Churn

Insight
This chart compares the average watch time of churned and retained users.
![Watch Time vs Churn](https://raw.githubusercontent.com/KanzadaNur/Churn-Prediction/main/images/distrb_watch_h.png)
Key findings:

Churned users generally show lower engagement levels.

Higher watch time correlates with lower churn probability.

Business Implication

User engagement is a key retention driver.

Possible strategies:

Personalized recommendations

Content notifications

Engagement campaigns

📊 Mobile Usage vs Churn

Insight

This chart analyzes churn behavior among mobile-heavy users.
![Mobile Usage vs Churn](https://raw.githubusercontent.com/KanzadaNur/Churn-Prediction/main/images/distrub_mobile_churn.png)
Key findings:

Users who primarily access the platform through mobile devices may show higher churn likelihood.

Mobile usage patterns could indicate more casual engagement.

Business Implication

Improving the mobile experience and sending targeted mobile notifications could reduce churn risk.

📊 Correlation Heatmap

Insight
The heatmap shows relationships between numerical variables in the dataset.
![Boxplot and correlation](https://raw.githubusercontent.com/KanzadaNur/Churn-Prediction/main/images/boxplot_avg_watch_h.png)

Key observations:

Tenure and watch time show moderate correlation.

Engagement-related variables are important predictors of churn behavior.

No severe multicollinearity is present, making the dataset suitable for regression models.

🤖 Predictive Modeling
Logistic Regression – Churn Prediction

A logistic regression model was built to estimate churn probability.

Model preparation steps included:

Feature scaling

Train-test split

Stratification

Class balancing

Key Predictors of Churn

Based on model coefficients, the most influential features include:

User tenure

Average watch time

Engagement metrics

Users with lower tenure and lower engagement levels show higher churn risk.

📈 Linear Regression – Watch Time Analysis

A linear regression model was used to explore factors influencing watch time.

Key insights:

Longer tenure correlates with increased engagement.

Behavioral indicators significantly influence watch time.

Engagement is influenced by additional external factors not included in the dataset.

🧠 Business Insights

The analysis identifies several high-risk customer segments:

🔴 New users with low tenure
🔴 Users with low watch time
🔴 Users who have not received promotional offers
🔴 Mobile-heavy users with low engagement

📌 Recommendations

Retention teams should focus on:

Early lifecycle engagement programs

Personalized content recommendations

Targeted promotions for low-engagement users

Improved mobile user experience

🚀 Future Improvements

Possible extensions of this project include:

ROC-AUC model evaluation

Additional models (Random Forest, XGBoost)

Feature importance visualization

Customer lifetime value analysis

📂 Repository Structure
Churn-Prediction
│
├── Week3.ipynb
├── stream_works_user_data.csv
├── README.md
│
└── images/
    churn_distribution.png
    promo_vs_churn.png
    watch_time_vs_churn.png
    mobile_users_churn.png
    correlation_heatmap.png
👤 Author

Data analysis project focused on applying statistical analysis and machine learning techniques to identify drivers of customer churn and generate actionable business insights.
