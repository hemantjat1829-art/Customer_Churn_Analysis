 📊 Churn Analysis and Customer Intelligence

 📌 Project Overview

This project focuses on Customer Churn Analysis and Customer Intelligence using Python, Pandas, SQLite, Matplotlib, and Seaborn. The goal is to analyze customer subscription behavior, understand churn patterns, evaluate customer retention, and identify factors associated with customer churn.

The project transforms raw customer, subscription, and customer support data into a structured dataset for exploratory data analysis (EDA), KPI calculation, and visualization.

 🎯 Objectives

- Clean and preprocess raw customer and subscription data.
- Integrate customer, subscription, and support datasets.
- Calculate key business metrics related to churn and retention.
- Analyze churn across subscription plans and states.
- Evaluate revenue at risk and average revenue per user (ARPU).
- Explore relationships between customer churn, support escalations, and churn risk.
- Visualize trends and patterns to support data-driven decision-making.

 🛠️ Technologies Used

- Python — Data analysis and feature engineering
- Pandas — Data manipulation and data cleaning
- NumPy — Numerical operations and conditional logic
- SQLite — Database creation and data integration
- Matplotlib — Data visualization
- Seaborn — Statistical visualization and correlation analysis
- Jupyter Notebook — Interactive analysis and documentation

 🔄 Project Workflow

 1. Data Import and Database Integration
- Imported raw data from Excel worksheets.
- Created an SQLite database named `customer_churn.db`.
- Stored individual worksheets as separate database tables.
- Retrieved database tables into Pandas DataFrames.

 2. Data Cleaning and Preprocessing
- Renamed columns for better readability.
- Removed unnecessary columns.
- Converted date columns to appropriate datetime formats.
- Standardized gender values.
- Handled missing country values using state-to-country mapping.
- Removed unnecessary columns from customer support data.

 3. Feature Engineering
Created additional analytical features, including:

- Churn Flag: Identifies customers with a recorded cancellation date.
- Complaint Count: Calculates the number of support complaints per customer.
- Customer Tenure: Measures subscription duration in days.
- Churn Risk: Classifies customers into low, medium, and high risk categories using churn scores.
- Escalation Encoding: Converts escalation values into numeric form for correlation analysis.

 4. Data Integration
- Merged customer, subscription, and support datasets using customer IDs.
- Investigated duplicate customer records in support data.
- Aggregated complaint counts before retaining the latest support record per customer.
- Exported the integrated dataset to `exported_churn_data.csv`.

 5. Exploratory Data Analysis
Calculated key business metrics:

- Overall churn rate
- Customer retention rate
- Churn rate by subscription plan
- Average Revenue Per User (ARPU)
- Average customer tenure
- Revenue at risk from churned customers
- Support escalation rate
- Average complaints per customer
- Correlation between escalations and churn

 6. Data Visualization
Used Matplotlib and Seaborn to explore customer behavior through:

- Monthly churn trend analysis
- Churn rate by subscription plan
- Churn rate by state
- Correlation heatmaps
- Pair plots
- Categorical comparisons of monthly charges, gender, plan type, and churn risk
- Pivot tables for aggregated business metrics

 📈 Key Business Metrics

| Metric | Purpose |
|---|---|
| Churn Rate | Measures the percentage of customers who churned |
| Retention Rate | Measures the percentage of customers retained |
| ARPU | Measures average monthly charges per customer |
| Average Tenure | Measures the average subscription duration |
| Revenue at Risk | Estimates monthly charges associated with churned customers |
| Escalation Rate | Measures the proportion of records with escalated support cases |
| Average Complaints | Measures support complaints per unique customer |

 📂 Project Structure

```text
churn-analysis/
│
├── churn_analysis.ipynb
├── customer_churn_data_raw.xlsx
├── customer_churn.db
├── exported_churn_data.csv
└── README.md
```

Note: The Excel file is the notebook's input. The SQLite database and CSV file are generated during execution and should be included in the repository only if you intend to distribute those artifacts.

 🚀 How to Run the Project

 Prerequisites
Install Python and Jupyter Notebook.

 1. Clone the Repository

```bash
git clone <your-repository-url>
cd churn-analysis
```

 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn openpyxl jupyter
```

SQLite support is available through Python's standard library in typical Python installations.

 3. Add the Dataset

Place `customer_churn_data_raw.xlsx` in the project directory. The notebook expects this filename in its current working directory.

 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `churn_analysis.ipynb` and execute the cells in order.

 💡 Skills Demonstrated

- Data cleaning and preprocessing
- SQL and SQLite database operations
- Data integration and joins
- Feature engineering
- Exploratory data analysis
- KPI development and business analysis
- Data visualization
- Correlation analysis
- Customer churn and retention analysis

 🔮 Potential Improvements

- Build an interactive churn dashboard using Power BI.
- Add deeper churn comparisons by contract type and customer demographics.
- Investigate the relationship between support complaints and churn.
- Develop a predictive churn model using machine learning.
- Create actionable customer retention recommendations.
- Add automated data validation and a reproducible analysis pipeline.

 👨‍💻 Author

Hemant Jat

B.Tech in Computer Science Engineering | IIIT Vadodara

GitHub: [Your GitHub Profile](https://github.com/hemantjat1829-art)

LinkedIn: [Connect with me](https://www.linkedin.com/in/hemant-jat-431bab338/)

---

This project demonstrates a practical data analytics workflow, from raw data preparation and database integration to business KPI analysis and visualization.
