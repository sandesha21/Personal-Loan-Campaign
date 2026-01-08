# Personal Loan Campaign

## Overview  
This project focuses on predicting which existing bank customers are most likely to purchase a personal loan. By leveraging customer demographic, financial, and behavioral data, the project aims to support the marketing team in designing targeted campaigns, improving conversion rates, and increasing revenue from loan products.

## Objective  
The main objective was to build a predictive model that identifies potential customers who are likely to accept a personal loan offer. By analyzing key attributes such as income, credit card spending, account balance, and online banking usage, the project provides actionable insights to optimize marketing strategies and customer engagement.

## Dataset  
- **Source:** AllLife Bank customer data (educational project)  
- **Size:** 5,000 customer records  
- **Key Features:**  
  - Demographic details (age, education, family size)  
  - Financial behavior (income, mortgage, credit card usage)  
  - Banking behavior (online activity, existing products)  
- **Target:** Personal Loan Acceptance (`1` = Accepted, `0` = Not Accepted)
- **Class Distribution:** 9.6% positive cases (loan accepted)

## Installation
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Usage
```bash
jupyter notebook AIML_ML_Project_full_code_notebook.ipynb
```

## Project Structure
```
├── AIML_ML_Project_full_code_notebook.ipynb  # Main analysis notebook
├── Loan_Modelling.csv                        # Dataset
├── Loan_Modelling copy.csv                   # Dataset backup
├── README.md                                 # Project documentation
└── LICENSE                                   # License file
```

## Workflow  
1. **Data Preprocessing** – Cleaned and prepared the data by handling missing values, encoding categorical features, and feature engineering
2. **Exploratory Data Analysis (EDA)** – Explored relationships between customer attributes and loan acceptance using visualizations and statistical analysis  
3. **Model Development** – Built and evaluated Decision Tree classification models with hyperparameter tuning
4. **Model Optimization** – Applied pre-pruning and post-pruning techniques to improve generalization
5. **Insights & Recommendations** – Identified key drivers of loan adoption and provided actionable business recommendations

## Model Performance
### Best Model: Decision Tree (sklearn default)
- **Accuracy:** 98.6%
- **Precision:** 92.7%
- **Recall:** 93.3%
- **F1-Score:** 93.0%

### Model Comparison (Test Set Performance)
| Model | Accuracy | Recall | Precision | F1-Score |
|-------|----------|--------|-----------|----------|
| Decision Tree (Default) | 98.6% | 93.3% | 92.7% | 93.0% |
| Decision Tree (Pre-Pruning) | 77.9% | 100.0% | 31.0% | 47.4% |
| Decision Tree (Post-Pruning) | 77.9% | 100.0% | 31.0% | 47.4% |

## Key Insights & Findings
- **High-income customers** with annual income >$100k show significantly higher loan acceptance rates
- **Credit card spending** (CCAvg) is a strong predictor - customers spending >$3k monthly are prime targets
- **Education level** positively correlates with loan acceptance (Graduate/Advanced degree holders)
- **CD Account holders** demonstrate 60% higher conversion rates than non-holders
- **Age group 30-40** represents the optimal target demographic for personal loans
- **Family size** of 2-3 members shows higher loan uptake compared to single-member households

## Business Recommendations
1. **Target High-Value Segments:** Focus marketing on customers with income >$100k and high credit card spending
2. **Cross-Selling Strategy:** Leverage existing CD account holders for loan campaigns
3. **Age-Specific Campaigns:** Design targeted offers for 30-40 age group tied to life events
4. **Education-Based Messaging:** Create specialized campaigns for graduate-level customers
5. **Digital Channel Optimization:** Prioritize online banking users for digital loan applications

## Tech Stack  
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Tools:** Jupyter Notebook / Google Colab  
- **Models:** Decision Tree Classifier with hyperparameter tuning

## Future Enhancements
- Implement ensemble methods (Random Forest, XGBoost) for improved accuracy
- Develop real-time prediction API for loan approval systems
- A/B testing framework for campaign optimization
- Advanced feature engineering with external data sources
- Deep learning models for complex pattern recognition

## Data Privacy
This project uses anonymized customer data for educational purposes only. All personal identifiers have been removed to ensure privacy compliance.

## Author  
**Sandesh S. Badwaik**  
- [LinkedIn](https://www.linkedin.com/in/sbadwaik/)
