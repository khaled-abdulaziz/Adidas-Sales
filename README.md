# 👟 Adidas US Sales Analysis & Prediction

A data science project analyzing Adidas US sales data (2020–2021) covering exploratory data analysis, statistical hypothesis testing, and machine learning prediction of total sales.

----

## 📊 Dataset

- **Source:** [Kaggle — Adidas US Sales Dataset](https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset)
- **Size:** 9,648 records × 13 columns
- **Period:** 2020 – 2021
- **Key columns:** Retailer, Region, State, City, Product, Price per Unit, Units Sold, Total Sales, Operating Profit, Sales Method

---

## 🔍 Project Highlights

### Exploratory Data Analysis (EDA)
- Analyzed sales trends over time (monthly, yearly, by weekday)
- Compared performance across 5 regions: Northeast, South, West, Midwest, Southeast
- Explored 6 retailers: Foot Locker, Walmart, Sports Direct, West Gear, Kohl's, Amazon
- Reviewed 6 product categories across Men's and Women's lines

### Statistical Testing
- **T-test (West vs. Northeast regions):** Found a statistically significant difference in sales (p < 0.05), with the West region outperforming the Northeast
- **T-test (In-store vs. Outlet):** Compared sales distribution across sales channels

### Machine Learning — Total Sales Prediction
- Model: **Random Forest Regressor**
- Preprocessing: One-Hot Encoding for categorical features, MinMax Scaling
- Tuning: GridSearchCV with 5-fold cross-validation
- Metrics reported: R², MAE, MSE

---

## 📁 Project Structure

```
adidas-sales-analysis/
│
├── addidas_sales.ipynb           # Main notebook (EDA + stats + ML)
├── Adidas US Sales Datasets.xlsx # Dataset
└── README.md
```

---

## ▶️ How to Run

1. Clone the repository
```bash
git clone https://github.com/your-username/adidas-sales-analysis.git
```
2. Install the required libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
```
3. Open the notebook in Jupyter
```bash
jupyter notebook addidas_sales.ipynb
```
4. Make sure `Adidas US Sales Datasets.xlsx` is in the same folder as the notebook, then run all cells

---

## 📦 Libraries Used

| Library | Purpose |
|---|---|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` / `seaborn` | Data visualization |
| `scipy.stats` | Statistical hypothesis testing |
| `scikit-learn` | Machine learning (Random Forest, GridSearchCV, scaling) |

---

## 💡 Key Findings

- **Total revenue across dataset:** ~$900M
- The **West region** generates significantly higher sales than the Northeast (confirmed by T-test)
- **Online sales** are growing but in-store remains the dominant channel by transaction volume
- **Men's Street Footwear** is the top-performing product category
- Random Forest with hyperparameter tuning achieved strong predictive performance on Total Sales

---

## 👤 Author

**Khaled Abdulaziz**
