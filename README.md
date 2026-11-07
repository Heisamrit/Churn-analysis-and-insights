# 📊 Customer Churn Analysis & Insights

## 📌 Project Overview

Customer Churn Analysis is a data analytics project focused on understanding customer behavior, identifying churn patterns, and generating actionable business insights.

The project uses Python, SQL (SQLite), and data visualization libraries to analyze customer, subscription, and customer support data.

The main objective is to identify customers who are likely to leave, understand the factors associated with customer churn, and help businesses improve customer retention strategies.

## 🎯 Project Objectives

- Analyze customer churn and retention rates.
- Identify churn patterns across different subscription plans.
- Understand customer behavior based on subscription types.
- Analyze churn distribution across different states.
- Calculate revenue at risk from churned customers.
- Explore the relationship between customer support escalations and churn.
- Categorize customers into different churn risk levels.
- Generate meaningful business insights through data visualization.

## 🛠️ Technologies & Tools Used

| Technology | Purpose |
|---|---|
| Python | Data analysis and processing |
| SQL | Data extraction and database operations |
| SQLite | Database management |
| NumPy | Numerical operations and feature engineering |
| Pandas | Data cleaning and manipulation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Interactive analysis |

## 📂 Dataset Description

The project uses three primary database tables:

**1. Customer Table**
- Customer ID
- Customer Name
- Country
- State
- Gender
- Date of Birth
- Customer Interests

**2. Subscription Table**
- Customer ID
- Subscription Start Date
- Subscription Type
- Renewal Date
- Plan Type
- Contract Type
- Cancellation Date
- Cancellation Reason
- Monthly Charges
- Customer Lifetime Value (CLTV)
- Churn Score

**3. Customer Support Table**
- Customer ID
- Complaint Date
- Escalations
- CSAT Score
- Customer Comments

## 🔄 Project Workflow

### 1. Data Extraction
- Connected Python to SQLite database.
- Retrieved database tables using SQL queries.
- Loaded tables into Pandas DataFrames.

### 2. Data Cleaning & Preprocessing
- Renamed columns for consistency.
- Removed unnecessary columns.
- Converted date columns into datetime format.
- Standardized gender values.
- Handled missing values in the country column.
- Cleaned customer support and subscription data.

### 3. Feature Engineering
- Created a `churn_flag` column using cancellation dates.
- Merged customer, subscription, and support datasets.
- Calculated complaint counts.
- Created customer churn risk categories:
  - Low Risk
  - Medium Risk
  - High Risk

### 4. Exploratory Data Analysis (EDA)
- Overall churn rate.
- Customer retention rate.
- Churn by plan type.
- Churn by subscription type.
- Churn by state.
- Revenue at risk.
- Correlation between escalations and churn.

### 5. Data Visualization
Created visualizations using Matplotlib and Seaborn:

- Monthly churn trend.
- Churn by subscription plan.
- Churn by state.
- Correlation heatmap.
- Pair plot.
- Categorical comparison plots.
- Pivot table analysis.

## 📈 Key Business Insights

The following results were obtained from the analyzed dataset:

| Analysis | Result |
|---|---:|
| Overall Churn Rate | 28.57% |
| Customer Retention Rate | 71.43% |
| Basic Plan Churn | 60.00% |
| Standard Plan Churn | 22.22% |
| Premium Plan Churn | 14.29% |
| Referral Subscription Churn | 83.33% |
| Paid Subscription Churn | 16.67% |
| Organic Subscription Churn | 0.00% |
| Escalations & Churn Correlation | 0.77 |

### 💡 Business Recommendations

1. **Improve Basic Plan Retention:** Investigate why Basic plan customers have a higher churn rate and consider improving their subscription experience.

2. **Analyze Referral Customers:** Investigate the high churn observed among referral subscribers and review the quality of referral acquisition.

3. **Improve Customer Support:** Monitor escalations and customer satisfaction to identify potential churn risks.

4. **Monitor Churn Risk:** Use churn score categories to prioritize customer retention activities.

5. **Track Revenue at Risk:** Monitor revenue associated with cancelled subscriptions to understand the financial impact of churn.

*Note: These are exploratory findings from the available dataset. The dataset is small, so results should not be generalized without further validation.*

## 🚀 How to Run This Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Customer-Churn-Analysis.git
```

### Step 2: Navigate to the Project Directory

```bash
cd Customer-Churn-Analysis
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Notebook

Open `churn_analysis.ipynb` and execute the cells sequentially.

**Note:** The SQLite database file `churn.db` must be available in the project directory for the notebook to run successfully.

## 📌 Project Outcomes

- Developed an end-to-end customer churn analysis workflow.
- Gained practical experience with SQL and Python integration.
- Performed data cleaning, preprocessing, and feature engineering.
- Identified customer churn patterns and potential retention opportunities.
- Generated business insights through exploratory data analysis.
- Practiced data visualization and statistical analysis.

## 👨‍💻 Author

**Amrit Saini**

- GitHub: https://github.com/Heisamrit
- LinkedIn: https://www.linkedin.com/in/heisamrit

---

⭐ If you find this project useful, consider giving the repository a star!
