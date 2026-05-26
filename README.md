# Data Cleaning & Visualization Project
### Thiranex Internship — Task 1

---

## 📌 Project Overview

This project demonstrates end-to-end **data preprocessing and visualization** using Python.  
A raw dataset with real-world issues (missing values, duplicates, outliers) is cleaned and then analyzed through multiple visualizations.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `pandas` | Data manipulation & cleaning |
| `numpy` | Numerical operations |
| `matplotlib` | Core plotting |
| `seaborn` | Statistical visualizations |

---

## 📁 Project Structure

```
data_cleaning_project/
│
├── data/
│   ├── raw_dataset.csv        # Original dataset with injected issues
│   └── cleaned_dataset.csv    # Final clean dataset
│
├── outputs/
│   ├── 01_data_quality_report.png
│   ├── 02_distribution_analysis.png
│   ├── 03_department_city_insights.png
│   ├── 04_correlation_heatmap.png
│   └── 05_outlier_comparison.png
│
├── data_cleaning_visualization.py   # Main script
├── requirements.txt
└── README.md
```

---

## 🔧 Steps Performed

### 1. Raw Data Issues (Intentionally Injected)
- ❌ **Missing Values** — 15–32 nulls across Age, Salary, Department, Rating, etc.
- ❌ **Duplicate Rows** — 10 duplicate records added
- ❌ **Outliers** — Extreme values: Salary=500,000, Age=150, PurchaseAmount=9,999

### 2. Data Cleaning
- ✅ Removed **duplicate rows**
- ✅ Handled **outliers** using IQR (Interquartile Range) method
- ✅ Filled **missing values** — median for numeric, "Unknown" for categorical
- ✅ Corrected **data types** (int for Age, Rating)

### 3. Visualizations Generated
| # | Chart | Insight |
|---|-------|---------|
| 1 | Data Quality Report | Missing values heatmap, duplicate & row counts |
| 2 | Distribution Analysis | Age, Salary, Purchase Amount, Rating histograms |
| 3 | Department & City Insights | Avg salary by dept, purchase share by city |
| 4 | Correlation Heatmap | Relationships between numeric features |
| 5 | Outlier Comparison | Boxplots before vs after cleaning |

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/data-cleaning-visualization.git
cd data-cleaning-visualization

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the script
python data_cleaning_visualization.py
```

All output charts will be saved in the `outputs/` folder.

---

## 📊 Sample Output

**Before Cleaning:** 210 rows | 10 duplicates | 120 missing values  
**After Cleaning:** 152 rows | 0 duplicates | 0 missing values

---
