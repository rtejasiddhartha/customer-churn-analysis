# Customer Churn Analysis & Risk Segmentation Platform

## 📌 Project Overview
Customer churn is a critical challenge across subscription-based and service-driven industries such as SaaS platforms, telecom providers, OTT streaming services, and digital products.

This project simulates a real-world churn analytics use case for a **generic subscription-based service company**. Using a **synthetic but business-realistic dataset from Kaggle**, the project builds an end-to-end churn analysis and risk segmentation pipeline to identify churn drivers, predict churn risk, and recommend actionable retention strategies.

The final output is a **production-ready, customer-level dataset** designed for direct consumption by BI tools or business teams.

---

## 🎯 Business Objective
- Identify customers at high risk of churn
- Understand behavioral and operational churn drivers
- Segment customers by churn risk
- Recommend targeted retention actions
- Enable proactive, data-driven decision-making

---

## 📊 Dataset Description
- **Source:** Kaggle (Synthetic dataset)
- **Nature:** Business-realistic, rule-driven synthetic data
- **Records:** ~10,000 customers
- **Target Variable:** `churn` (0 = No, 1 = Yes)

The dataset is synthetically generated for educational and portfolio purposes.  
While it does not represent real customer data, it closely mirrors real-world churn patterns through realistic feature relationships and probabilistic labeling.

---

## 🏢 Industry Context & Applicability
Although the dataset is synthetic, it reflects common churn drivers observed in real-world subscription businesses.

This churn analytics framework is applicable across multiple industries, including:

- **SaaS & Cloud Platforms**
  - User engagement, feature usage, subscription fees, renewals
- **Telecom Services**
  - Contract types, billing behavior, support interactions
- **OTT & Streaming Platforms**
  - Login frequency, session duration, content engagement, inactivity
- **FinTech & Digital Products**
  - Usage trends, payment failures, customer support
- **EdTech & E-learning Platforms**
  - Platform activity, session duration, feature adoption

The analytical approach and modeling logic are **industry-agnostic** and can be adapted to real-world datasets with minimal changes.

---

## 🧠 Approach & Methodology

### 1. Data Preparation
- Loaded and validated customer-level data
- Handled missing values using business-safe defaults
- Ensured one record per customer
- Reviewed data distributions and statistical summaries

### 2. Exploratory Data Analysis (EDA)
- Analyzed churn distribution and confirmed class imbalance
- Studied engagement, inactivity, support, and billing patterns
- Identified key behavioral indicators of churn
- Performed outlier analysis using the IQR method

### 3. Feature Selection & Modeling
- Selected relevant engagement, support, and billing features
- Encoded categorical variables
- Applied feature scaling
- Trained a **Logistic Regression** model with class imbalance handling
- Generated churn probability scores

### 4. Threshold Tuning & Evaluation
- Applied a probability threshold (0.4) to balance recall and operational feasibility
- Evaluated performance using precision, recall, and F1-score
- Validated results on unseen test data

### 5. Risk Segmentation & Business Logic
- Segmented customers into **Low**, **Medium**, and **High** churn-risk groups using rule-based logic
- Combined ML predictions with risk segments
- Mapped customers to recommended retention actions

### 6. Production Simulation
- Applied the trained model to the full dataset
- Generated churn scores, risk segments, and actions for all customers
- Created a final BI-ready output table

---

## 📈 Key Insights
- Customers flagged for immediate retention actions showed the highest actual churn rates
- Lower engagement and higher inactivity strongly correlated with churn
- Support issues and payment failures were consistent churn drivers
- Risk segmentation aligned well with actual churn outcomes
- Churn risk was effectively concentrated into actionable customer groups

---

## 📤 Final Output
A consolidated customer-level dataset including:
- Churn probability (ML output)
- Churn prediction (threshold-based)
- Risk segment (business logic)
- Recommended retention action

This dataset is suitable for dashboards, reporting, and operational workflows.

---

## 🛠️ Tools & Technologies
- **Python:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (Logistic Regression)
- **Environment:** Jupyter Notebook
- **Version Control:** Git & GitHub
- **BI & Reporting:** Power BI

---

## 📌 Project Status & Next Steps
- Core analytics and modeling completed
- Final churn scoring dataset exported
- Power BI dashboards added as a visualization layer
- Advanced modeling and explainability can be added as optional extensions

---

## 👤 Author

**R. Teja Siddhartha**

- 💼 LinkedIn: https://linkedin.com/in/rtejasiddhartha  
- 💻 GitHub: https://github.com/rtejasiddhartha  
- 📧 Email: rtejasiddhartha18@gmail.com  

--- 
