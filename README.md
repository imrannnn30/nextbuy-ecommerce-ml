# NextBuy — E-Commerce Analytics & ML

> Data analysis and machine learning over 5 e-commerce datasets — answering 8 business questions and training 2 production-grade predictive models.

[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-dashboard-FF4B4B?style=flat&logo=streamlit&logoColor=white)](https://streamlit.io/)

## What it is

Full data pipeline on a multi-table e-commerce dataset (orders, products, departments, aisles, order_products). The project answers **8 business questions** through EDA, then trains **2 machine learning models**: an association-rules engine for product recommendations, and a RandomForest regressor for department-level performance prediction.

## Stack

| Layer            | Technology                                  |
| ---------------- | ------------------------------------------- |
| **Analysis**     | pandas, numpy, matplotlib, seaborn          |
| **ML — Model 1** | Apriori (mlxtend) — association rules       |
| **ML — Model 2** | scikit-learn RandomForest (300 estimators)  |
| **Dashboards**   | Streamlit (one per model)                   |
| **Notebooks**    | Jupyter for exploration & model development |

## Business questions answered

1. Top 10 best-selling products
2. Top 10 least-sold products by day of the week
3. Top 10 products added first to the cart
4. Top 10 products co-added with the most popular item
5. Top 10 most reordered products
6. When do customers usually order (by day)
7. Which department offers the fewest products
8. Sales by department × day of the week (heatmap)

## Models

### Model 1 — Product recommendation

- **Algorithm** : Apriori association rules mining
- **Metrics** : Support, Confidence, Lift
- **Use case** : suggest complementary products based on current cart

### Model 2 — Department efficiency prediction

- **Algorithm** : RandomForest Regressor (300 estimators)
- **Performance** : **R² = 0.990**, MAE = 0.101, RMSE = 0.219
- **Use case** : predict department performance by day of the week
- Models serialized to `.pkl` for dashboard consumption

## What I learned

- **End-to-end ML pipeline** — from raw CSV to trained model to deployed Streamlit dashboard
- **Hyperparameter tuning** to push RandomForest to R²=0.99 without overfitting
- **Association rules** beyond cosine similarity — when Apriori actually outperforms collaborative filtering for product-bundling
- **Notebook hygiene** — keeping `main.ipynb` and `model.ipynb` separated by concern (EDA vs. model dev)
- **Communicating findings** — every question gets a chart and a written interpretation, not just the number

## Project context

- **Year** : 2025–2026
- **School** : Epitech Bachelor, Mulhouse
- **Team** : 2 members
- **Course** : Data Analysis (B-DAT-201)

## Note

This is a portfolio summary. The full source code, notebooks, and trained models are private per Epitech academic policy. Available on request for recruiters.

---

[Imran Nogueira](https://github.com/imrannnn30)
