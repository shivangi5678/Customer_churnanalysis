# 📊 Telecom Customer Churn Analysis & Prediction

An end-to-end Data Analytics and Machine Learning project designed to identify high-risk customer churn patterns, understand churn drivers, and build predictive pipelines to support proactive customer retention.

---

## 📌 Project Overview
Customer retention is critical for telecom profitability. This project analyzes **7,043 customers** to identify key behavior patterns leading to churn, builds predictive models using Machine Learning, evaluates explainability using **SHAP**, and surfaces strategic insights via an interactive **Power BI Dashboard** and **SQL analysis**.

---

## 🎯 Key Business Insights
* **Overall Churn Rate**: Out of 7,043 customers, **1,869 (26.54%)** churned.
* **Contract Risk**: Month-to-month contracts exhibit the highest churn rate (~42.7%), whereas 2-year contracts show strong retention (churn < 3%).
* **Tenure Impact**: Customers in their first 12 months (0–12m) are at the highest risk of churn.
* **Service Type**: Fiber Optic users and Electronic Check payers account for a significant share of churned accounts due to pricing and service friction.

---

## 🛠️ Tech Stack & Tools
* **Python**: Pandas, NumPy, Scikit-Learn, SHAP, Seaborn, Matplotlib
* **Database & Querying**: SQLite / SQL
* **BI & Visualization**: Power BI
* **Environment**: Google Colab / Jupyter Notebook

---

## 📈 Machine Learning Workflow

1. **Data Preprocessing & Cleaning**:
   * Converted `Total Charges` to numeric, handled missing values, and engineered features (`Total Services`, `Tenure Groups`).
   * Addressed data leakage by removing non-predictive attributes (IDs, coordinates, churn labels/reasons).

2. **Model Evaluation & Comparison**:
   * Evaluated multiple algorithms including **Logistic Regression**, **Decision Trees**, **Random Forest**, and **Gradient Boosting**.
   * **Best Model**: **Gradient Boosting Classifier** (ROC-AUC: `0.8523`, Accuracy: `~80.2%`).

3. **Customer Segmentation & Risk Scoring**:
   * Generated Churn Probabilities and segmented users into **Low Risk**, **Medium Risk**, and **High Risk**.
   * Applied **K-Means Clustering** to identify 4 core customer personas (e.g., *Long-term High-Value*, *Budget/Low-Usage*).
   * Used **SHAP (SHapley Additive exPlanations)** to interpret model predictions and feature importance.

---

## 📊 Dashboard Preview
The interactive Power BI dashboard compares overall customer demographics and behavior directly against the churned customer segment.

* **Total Customers Analyzed**: 7.043K
* **Total Churners**: 1.869K
* **Key Dimensions Tracked**: Demographics, Tenure Bins, Internet Service Types, Payment Methods, and Contract Types.

---

## 🚀 How to Run

1. **Clone the repository**:
   ```bash
   git clone [https://github.com/shivangi5678/Customer_churnanalysis.git](https://github.com/shivangi5678/Customer_churnanalysis.git)
   cd Customer_churnanalysis
