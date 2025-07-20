# HR-Analytics---Predict-Employee-Attrition

A comprehensive HR Analytics project to explore, model, and visualize employee attrition patterns using Python, SHAP, and Power BI.

## Repository Structure
<img width="709" height="594" alt="image" src="https://github.com/user-attachments/assets/65d695ec-5e73-4e66-ae60-55e3185209e4" />


## Tools & Technologies

- **Python**: Pandas, Seaborn, Matplotlib, Scikit-learn
- **SHAP**: Model interpretability & explainability
- **Power BI**: Dashboard and stakeholder-facing visualizations
- **Google Colab**: Analysis and model development

## Exploratory Data Analysis (EDA)

Key insights uncovered:
- High attrition in **Sales** and **R&D** departments.
- Younger employees (age 25–35) and **low salary bands** showed higher attrition.
- Employees with frequent **OverTime** and **BusinessTravel** were more likely to resign.
- Attrition rate is highest among employees with **0–3 years at company**.

Correlation matrix, boxplots, and bar charts were used for trend identification.

## Machine Learning Models

Two classification models were trained:
1. **Logistic Regression** (Baseline)
2. **Decision Tree Classifier** (max_depth=5)

Evaluation Metrics:
| Metric         | Logistic Regression | Decision Tree |
|----------------|---------------------|----------------|
| Accuracy       | ~87%                 | ~84%            |
| ROC AUC Score  | ~0.80                | ~0.66           |


## SHAP Explainability

SHAP (SHapley Additive exPlanations) was used to explain feature contributions.

Top influencing features:
- `OverTime`
- `MonthlyIncome`
- `JobRole`
- `Age`
- `YearsAtCompany`

## Power BI Dashboard

Includes bar chart visuals for:
- Attrition by **Department**, **Job Role**, **Age Group**, **Education**, **Gender**
- **Salary Ranges**, **Business Travel**, **OverTime**
- Interactive **slicers** for Department and Gender

### Key Recommendations:
- Improve **compensation** in low-paying roles.
- Reduce **overtime hours** and **travel frequency**.
- Provide career growth programs for early-tenure employees.
- Monitor high-risk job roles such as Sales Executives.
- Conduct regular **pulse surveys** and **exit interviews**.

