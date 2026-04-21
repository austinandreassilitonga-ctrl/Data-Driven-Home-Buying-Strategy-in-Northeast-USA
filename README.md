#  Data Driven Home Buying Strategy — Northeast States, USA

> A data analysis project to help **Mr. Andreas** find the right home within a **$2,000,000 USD** budget.

---

##  Background

Mr. Andreas is a 40-year-old married man with two children. He is planning to relocate and purchase a house in the Northeast States, USA. With savings of $2,000,000 USD, he needs data-driven guidance to avoid costly mistakes and find a home that truly fits his family's needs.

This project analyzes a housing dataset to answer critical questions about price distributions, market averages, outliers, and which features most influence price — all with Mr. Andreas' budget and family situation in mind.

---

##  Objectives

| # | Question |
|---|----------|
| 1 | How is housing price distributed across the dataset? |
| 2 | What percentage of homes fall within the $2M budget? |
| 3 | How many outliers exist and how do they affect the analysis? |
| 4 | What is the average market price of homes? |
| 5 | Are homes within the $2M range suitable for a family of four? |
| 6 | Which features (stories, bedrooms, amenities) most influence price? |

---

##  Repository Structure

```
├── README.md                    ← Project overview (this file)
├── notebook.ipynb               ← Main Jupyter Notebook with full analysis
├── Housing.csv                  ← Dataset (sourced from Kaggle)
├── description.md               ← Project metadata and stack summary
└── summary_dashboard.png        ← dashboard all visualization
```

---

##  Dataset

- **Source:** [Kaggle.com — Housing Prices Dataset](https://www.kaggle.com/)
- **Shape:** 545 rows × 13 columns
- **No missing values, no duplicates**

| Column | Description |
|--------|-------------|
| `price` | House price (USD) |
| `area` | Total area (sq ft) |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `stories` | Number of floors |
| `mainroad` | Located on main road (yes/no) |
| `guestroom` | Has guest room (yes/no) |
| `basement` | Has basement (yes/no) |
| `hotwaterheating` | Has hot water heating (yes/no) |
| `airconditioning` | Has air conditioning (yes/no) |
| `parking` | Number of parking spots |
| `prefarea` | Located in preferred area (yes/no) |
| `furnishingstatus` | furnished / semi-furnished / unfurnished |

---

##  Analysis Highlights

- **Price Distribution** — Histogram, KDE, and percentile bands
- **Outlier Detection** — IQR method with before/after comparison
- **Budget Feasibility** — % of homes within $2M, pie and bar charts
- **Feature Impact** — Scatter plots, boxplots, violin plots, grouped bar charts
- **Statistical Tests** — One-Way ANOVA, Kruskal-Wallis, Pearson correlation
- **Family-Suitable Filter** — Homes within budget with ≥ 3 bedrooms
- **Summary Dashboard** — 7-panel comprehensive visualization

---

##  Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical computations |
| `scipy` | Statistical tests (ANOVA, KDE, correlation) |
| `matplotlib` | All visualizations and dashboard |

---

##  Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/housing-price-analysis.git
cd housing-price-analysis
```

### 2. Install dependencies
```bash
pip install pandas numpy scipy matplotlib jupyter
```

### 3. Run the notebook
```bash
jupyter notebook notebook.ipynb
```

---

##  Key Results

| Metric | Value |
|--------|-------|
| Total listings | 545 |
| Mean price | ~$4.77M |
| Median price | ~$4.34M |
| Homes within $2M budget | ~14% |
| Family-suitable (budget + ≥3 beds) | varies by filter |
| Strongest price predictor (numeric) | Area (R² ≈ 0.28) |

---

## Dashboard
**Tableau Dashboard** : [Tableau](https://public.tableau.com/views/HousePriceDashboard-Austin/HOUSINGPRICEDASHBOARD?:language=en-US&publish=yes&:sid=9C0A97653A1441E6BD3B42207D091867-0:0&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

##  Recommendation

For Mr. Andreas, the analysis suggests focusing on **3-bedroom, semi-furnished homes priced between $1.5M and $2.0M**, preferably near the main road. These homes represent the best combination of affordability, space, and family suitability within the available market.

---

##  Author

**Austin Andreas Ezra Silitonga**

---

##  License

This project is for educational and analytical purposes only. Dataset is publicly available on Kaggle.
