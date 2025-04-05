
# 📦 Supplier Disruption Risk Prediction

[![R Markdown](https://img.shields.io/badge/Built%20With-R%20Markdown-75AADB?logo=rstudio)](https://rmarkdown.rstudio.com/)  
[![Status](https://img.shields.io/badge/Project-Complete-success)](https://github.com/snagori28)  
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 🎯 Project Objective

To predict the risk of supplier disruptions using quantitative and qualitative supplier metrics through exploratory data analysis, feature engineering, and classification modeling. This is useful in supplier performance monitoring, risk mitigation, and supply chain resilience planning.

---

## 🔍 Background & Motivation

Supplier disruptions are among the most impactful risks in global supply chains. Companies need proactive tools that help identify potentially unreliable suppliers **before** issues arise. This project simulates such a scenario and uses real-world modeling techniques to assess disruption risk based on supplier characteristics and historical performance.

---

## 📊 Dataset Overview

- **Location**: `data/Supplier_Disruption_Risk.csv`
- **No. of Observations**: ~100+
- **Target Variable**: `disruption_risk` (Binary: Yes/No)

---

## 🧬 Feature Descriptions

| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `supplier_id`            | Unique identifier for each supplier                                         |
| `financial_risk_score`   | Score (0-100) based on financial health                                     |
| `environmental_score`    | Score (0-100) reflecting ESG factors                                         |
| `geo_risk_rating`        | Geographic disruption risk (Low/Medium/High)                                |
| `previous_disruptions`  | Count of disruptions in the past 3 years                                     |
| `on_time_delivery_rate` | % of orders delivered on time                                                |
| `product_diversity`      | Count of distinct products supplied                                          |
| `years_of_relationship` | Duration of supplier engagement in years                                     |
| `disruption_risk`        | Binary label - whether the supplier was disrupted (Yes/No)                  |

---

## 🧮 Methodology

1. **Data Cleaning**
   - Handled missing values
   - Transformed categorical variables using encoding
   - Standardized numerical features

2. **Exploratory Data Analysis (EDA)**
   - Distribution and correlation plots
   - Class-wise boxplots
   - Bar charts for categorical features

3. **Feature Engineering**
   - Normalization
   - Derived variables (e.g., disruption frequency rate)

4. **Modeling**
   - Logistic Regression (Binary Classification)

5. **Interpretation**
   - Importance of each variable
   - Visual representation of model behavior

---

## 📈 Visualizations

Here are some key charts and visualizations created in the analysis:

- Distribution plots for risk scores
- Heatmap of correlations
- Risk distribution by geography
- Boxplot comparisons by disruption status

➡️ Full interactive report: `output/Supplier_Disruption_Risk.html`

---

## 🔍 Key Insights

- Financial and environmental scores are strong predictors of risk.
- Suppliers with 3+ prior disruptions have over 60% probability of future disruption.
- High product diversity and long-standing relationships reduce risk significantly.
- On-time delivery rate below 75% correlates with high disruption risk.

---

## 🖼️ Screenshots

| Screenshot Description                   | Preview |
|------------------------------------------|---------|
| Correlation Heatmap                      | ![](screenshots/correlation_heatmap.png) |
| Boxplot of Financial Risk vs Disruption  | ![](screenshots/boxplot_financial_score.png) |
| Logistic Regression Confusion Matrix     | ![](screenshots/confusion_matrix.png) |
| AUC-ROC Curve                            | ![](screenshots/roc_curve.png) |

---

## 🗂️ File Structure

```
Supplier_Disruption_Risk/
├── data/
│   └── Supplier_Disruption_Risk.csv
├── scripts/
│   └── Supplier_Disruption_Risk.Rmd
├── output/
│   └── Supplier_Disruption_Risk.html
├── screenshots/
│   └── correlation_heatmap.png
│   └── boxplot_financial_score.png
│   └── confusion_matrix.png
│   └── roc_curve.png
└── README.md
```

---

## 🛠️ Technologies Used

- **Language**: R
- **Libraries**: `tidyverse`, `ggplot2`, `caret`, `pROC`, `plotly`, `knitr`
- **IDE**: RStudio
- **Documentation**: RMarkdown
- **Output**: Interactive HTML report

---

## ▶️ How to Run

1. Clone the repository
2. Open `scripts/Supplier_Disruption_Risk.Rmd` in RStudio
3. Install required packages if not already installed
4. Knit the file to generate `output/Supplier_Disruption_Risk.html`
5. Explore visualizations and insights

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

- Inspired by real-world challenges in supplier and vendor management.
- Educational project for demonstrating predictive analytics using R.
