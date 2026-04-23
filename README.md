# 📊 DataLens: CSV Explorer & Visual Insights Dashboard

> **QSkill Python Development Internship — Slab 1, Task 1**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8%2B-orange)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.13%2B-4c72b0)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## 📌 Project Overview

**DataLens** is a data analysis and visualization project that demonstrates core data science skills using a simulated Indian retail sales dataset. The project loads a CSV file with **Pandas**, computes descriptive statistics and column averages, and produces three distinct visualizations using **Matplotlib** and **Seaborn** — each paired with actionable business insights.

---

## ✨ Features

- 📁 **CSV Loading** — Load and inspect any CSV dataset using Pandas
- 🔍 **Data Exploration** — Shape, dtypes, missing values, and statistical summary
- 📐 **Column Averages** — Revenue, Units Sold, Price, Rating, and Discount averages
- 📊 **Bar Chart** — Total revenue comparison across product categories
- 🔵 **Scatter Plot** — Relationship between units sold and revenue with trend line
- 🌡️ **Heatmap** — Average revenue grid across City × Category combinations
- 💡 **Insights** — Business observations derived from each visualization

---

## 🗂️ Project Structure

```
DataLens/
│
├── DataLens_CSV_Explorer.ipynb   # Main Jupyter Notebook (all steps)
├── retail_sales.csv              # Sample dataset (200 rows × 9 columns)
├── bar_chart.png                 # Visualization 1 output
├── scatter_plot.png              # Visualization 2 output
├── heatmap.png                   # Visualization 3 output
└── README.md                     # This file
```

---

## 📦 Dataset

A synthetic **Retail Sales Dataset** was generated with **200 transaction records** simulating Indian retail commerce across 6 major cities and 5 product categories.

| Column | Type | Description | Range |
|--------|------|-------------|-------|
| `City` | String | Indian metro city | Mumbai, Delhi, Bangalore, Hyderabad, Chennai, Kolkata |
| `Category` | String | Product category | Electronics, Clothing, Groceries, Furniture, Sports |
| `Units_Sold` | Integer | Units per transaction | 10 – 300 |
| `Price_Per_Unit` | Float | Price in Rupees | ₹50 – ₹5,000 |
| `Customer_Age` | Integer | Buyer age | 18 – 65 |
| `Rating` | Float | Customer satisfaction | 1.0 – 5.0 |
| `Discount_Pct` | Integer | Discount applied | 0 – 50 % |
| `Revenue` | Float | Derived column | Units × Price × (1 − Disc%) |

---

## 📊 Visualizations

### 1. Bar Chart — Total Revenue by Category
Compares total revenue (₹ millions) across all 5 product categories sorted in descending order.

**Key Finding:** Electronics leads all categories due to high price per unit, while Groceries generates the lowest revenue despite consistent demand volume.

### 2. Scatter Plot — Units Sold vs Revenue
Plots individual transactions as dots coloured by category, with a trend line overlay showing the overall correlation direction.

**Key Finding:** A clear positive correlation exists. Electronics and Furniture cluster high on the revenue axis even with few units — confirming their high price point advantage.

### 3. Heatmap — Average Revenue: City × Category
A pivot-table heatmap showing the mean revenue per City-Category combination. Darker cells indicate higher average revenue.

**Key Finding:** Mumbai and Delhi dominate across most categories. Furniture in Bangalore and Electronics in Hyderabad are strong regional performers.

---

## 💡 Key Insights

- **Electronics dominates** revenue — high unit prices drive value even at moderate volume.
- **Groceries** needs a pricing or bundling strategy to improve average revenue per transaction.
- **Mumbai and Delhi** are the top-performing cities across nearly all categories.
- **Average discount of ~25%** is significant — a data-driven discount policy could improve margins.
- **Outlier transactions** (high units + high revenue) may represent wholesale/B2B buyers worth targeting.

---

## 🧑‍💻 Tech Stack

| Tool | Version | Purpose |
|------|---------|---------|
| Python | 3.10+ | Core programming language |
| Pandas | 2.x | Data loading, cleaning & analysis |
| NumPy | 1.26+ | Numerical operations |
| Matplotlib | 3.8+ | Base plotting framework |
| Seaborn | 0.13+ | Statistical visualizations |
| Jupyter Notebook | 7.x | Interactive development environment |

---

## 📁 Output Files

| File | Description |
|------|-------------|
| `retail_sales.csv` | Generated sample dataset |
| `bar_chart.png` | Revenue by product category |
| `scatter_plot.png` | Units sold vs revenue scatter |
| `heatmap.png` | Avg revenue by city and category |

---

## 🎓 Internship Details

| Field | Details |
|-------|---------|
| Organization | QSkill |
| Domain | Python Development |
| Slab | Slab 1 (Beginners) |
| Task | Task 1 of 3 |
| Duration | 1st April 2026 – 1st May 2026 |

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

- Dataset inspired by real-world Indian retail commerce patterns
- Built as part of the **QSkill Python Development Internship — Slab 1**

---

*Made with ❤️ using Python, Pandas, Matplotlib & Seaborn*
