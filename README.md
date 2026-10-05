# E-Commerce Sales & Predictive Analytics

An end-to-end e-commerce analytics project combining **data analysis, machine learning, predictive analytics, Flask, Plotly, and Power BI** to analyze sales performance, predict sales, and classify order profitability.

## Project Overview

This project analyzes e-commerce order data to answer two business questions:

1. How can sales performance be analyzed across products, categories, regions, and other business dimensions?
2. Can machine learning be used to predict expected sales and identify whether an order is likely to be profitable?

The project combines a business analytics dashboard with predictive machine learning models in a Flask web application.

## Key Features

- E-commerce sales analysis and visualization
- Interactive Plotly charts
- Power BI dashboard for business reporting
- Sales prediction using **Random Forest Regression**
- Profitability classification using **Random Forest Classification**
- Categorical feature encoding
- Flask-based web application
- Persisted machine learning models using Pickle

## Machine Learning

### Sales Prediction

A **Random Forest Regressor** predicts `sales_per_order` using features such as:

- Product Category
- Customer Region
- Shipping Type
- Order Quantity
- Scheduled Shipping Days

### Profitability Prediction

A **Random Forest Classifier** predicts whether an order is profitable:

- `1` → Profitable
- `0` → Not Profitable

Categorical variables are encoded before being passed to the models.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Machine Learning | Scikit-learn, Random Forest |
| Visualization | Plotly |
| Dashboarding | Microsoft Power BI |
| Web Framework | Flask |
| Model Storage | Pickle |
| Development | Jupyter Notebook, VS Code |

## Project Architecture

```text
E-Commerce Dataset
        │
        ▼
Data Preparation & Processing
        │
        ├──────────────► Exploratory Analysis
        │                      │
        │                      ▼
        │                Plotly Visualizations
        │
        └──────────────► Machine Learning
                               │
                  ┌────────────┴────────────┐
                  ▼                         ▼
        Random Forest Regressor    Random Forest Classifier
                  │                         │
                  ▼                         ▼
          Sales Prediction         Profitability Prediction
                  │                         │
                  └────────────┬────────────┘
                               ▼
                        Flask Web Application

E-Commerce Dataset ──────────► Power BI Dashboard
```

## Project Structure

```text
ecommerce-sales-predictive-analytics/
│
├── app1.py
├── train_models.py
├── Ecommerce_data.csv
├── sales_model222.pkl
├── profit_model222.pkl
├── label_encoders222.pkl
├── Ecommerce.pbix
├── test.py
├── test_data.xlsx
├── Untitled.ipynb
│
├── templates/
│   └── ...
│
├── static/
│   └── ...
│
└── README.md
```

## Running the Flask Application

### 1. Clone the repository

```bash
git clone https://github.com/syednadeemuddin44/ecommerce-sales-predictive-analytics.git
cd ecommerce-sales-predictive-analytics
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install pandas numpy scikit-learn flask plotly openpyxl
```

### 4. Run the application

```bash
python app1.py
```

Open the local Flask URL shown in the terminal.

## Power BI Dashboard

The repository contains the Power BI report:

```text
Ecommerce.pbix
```

It provides interactive business analysis of the e-commerce dataset and complements the predictive analytics component.

## Business Value

The project demonstrates how historical e-commerce data can be transformed into actionable insights by combining:

- Descriptive analytics
- Data visualization
- Predictive modeling
- Profitability analysis
- Interactive dashboards

This can help businesses understand sales patterns, evaluate order profitability, and support data-driven decision-making.

## Skills Demonstrated

**Data Analytics:** Python, Pandas, NumPy, exploratory data analysis, data visualization

**Machine Learning:** Random Forest Regression, Random Forest Classification, feature encoding, predictive analytics

**Business Intelligence:** Power BI, interactive dashboards, business reporting

**Application Development:** Flask, Plotly, Python model integration

## Future Improvements

- Add formal model evaluation metrics and cross-validation
- Add feature importance analysis
- Compare Random Forest with other regression/classification algorithms
- Improve model validation and monitoring
- Deploy the Flask application
- Connect the application to a production database
- Add automated dashboard data refresh

## Author

**Syed Nadeemuddin**  
B.Tech Computer Science (Data Science)

- GitHub: https://github.com/syednadeemuddin44
- LinkedIn: https://www.linkedin.com/in/nadeem2004

---

*Portfolio project demonstrating e-commerce analytics, predictive modeling, and business intelligence workflows.*
