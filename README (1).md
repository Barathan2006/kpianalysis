# 👗 Fashion E-Commerce Sales Dashboard

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

**An end-to-end data analysis project on a fashion e-commerce dataset with KPI analysis, data cleaning, and sales dashboard visualization.**

</div>

---

## 📌 Project Overview

This project analyzes a **30,000+ row fashion e-commerce dataset** to uncover insights about brands, categories, pricing, and discounts. It includes full data cleaning, KPI calculation, and a visual sales dashboard.

---

## 📂 Project Structure

```
fashion-sales-dashboard/
│
├── 📓 fashion_analysis.ipynb     # Main Jupyter Notebook
├── 📊 FashionDataset.csv         # Raw dataset
├── 🖼️ fashion_dashboard.png      # Generated dashboard image
├── 📄 README.md                  # Project documentation
└── 📁 outputs/                   # Cleaned data & charts
```

---

## 🔍 Dataset Info

| Feature | Details |
|---|---|
| 📦 Total Records | 30,758 rows |
| 🏷️ Columns | BrandName, Details, Sizes, MRP, SellPrice, Discount, Category |
| 🧹 Missing Values | MRP (96%), Discount (96%), SellPrice (7 rows) |

---

## 🛠️ Data Cleaning Steps

- ✅ Dropped unnamed index column
- ✅ Converted `MRP`, `SellPrice`, `Discount` from object → float64
- ✅ Converted `BrandName`, `Category` → category dtype (memory optimized)
- ✅ Dropped 7 rows with missing `SellPrice`
- ✅ Filled missing `MRP` with `SellPrice`
- ✅ Recalculated `Discount` from MRP & SellPrice
- ✅ Fixed string `"Nan"` in `Sizes` column → `'Not Specified'`

---

## 📊 KPI Analysis

| KPI | Description |
|---|---|
| 💰 **Total Revenue** | Sum of all SellPrice values |
| 🛒 **Total Orders** | Count of all product rows |
| 📈 **AOV (Avg Order Value)** | Revenue ÷ Orders |
| 🏆 **Top Category** | Highest revenue-generating category |
| 🥇 **Top Brand** | Brand with maximum sales |

---

## 📸 Dashboard Preview

> 📌 Run the notebook to generate `fashion_dashboard.png`

The dashboard includes:
- KPI summary cards (Revenue, Orders, AOV)
- Revenue by Category (horizontal bar chart)
- Top 10 Brands by Revenue (bar chart)

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/fashion-sales-dashboard.git
cd fashion-sales-dashboard

# 2. Install dependencies
pip install pandas matplotlib

# 3. Launch Jupyter Notebook
jupyter notebook fashion_analysis.ipynb
```

---

## 🧰 Tech Stack

- **Python 3.8+**
- **Pandas** — Data manipulation & cleaning
- **Matplotlib** — Dashboard visualization
- **Jupyter Notebook** — Interactive analysis

---

## 💡 Key Insights

- 🏷️ **Western Wear** dominates the dataset in both volume and revenue
- 💸 MRP data is largely missing (~96%), so discount analysis is limited
- 👗 Jewellery has **higher AOV** compared to clothing categories
- 🔝 A small set of brands contribute to the majority of total sales

---

## 🙋 Author

**Your Name**
[![GitHub](https://img.shields.io/badge/GitHub-Barathan2006-black?style=flat&logo=github)](https://github.com/Barathan2006)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/your-profile)

---

## 📃 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
⭐ If you found this helpful, please consider giving it a star!
</div>
