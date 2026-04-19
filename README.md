
---

📌 Iowa Liquor Sales Analysis (20M+ Rows, DuckDB, Mixed Linear Models)

A large‑scale analytics project exploring 20 million+ retail liquor transactions from the State of Iowa.  
This project demonstrates advanced SQL engineering, statistical modeling, and data storytelling — turning raw, messy public data into clear, actionable insights.

---

🚀 Project Overview

This project analyzes how liquor sales vary across cities, months, and store density using:

- High‑performance SQL with DuckDB
- Statistical modeling with GEE and Mixed Linear Models
- Variance decomposition (ICC) to quantify city‑level effects
- Visual storytelling using Python and AI‑assisted graphics

The goal is to understand the structural drivers of sales and communicate insights in a stakeholder‑friendly way.

---

📊 Dataset

- Source: Iowa Department of Commerce (public dataset)
- Rows: 20M+
- Columns: Store info, city, category, bottle volume, sale amount, date, vendor, etc.
- Granularity: Individual retail transactions

This dataset is known for its size, real‑world messiness, and suitability for statistical modeling.

---

🧹 Data Cleaning & SQL Pipeline (DuckDB)

DuckDB was used to query tens of millions of rows directly from CSV files with excellent performance.

Key cleaning steps:

- Fixing mixed data types (numeric stored as VARCHAR)
- Parsing currency fields into floats
- Standardizing dates and extracting month/year
- Handling missing values
- Creating city‑level aggregates
- Building a reproducible SQL pipeline

This pipeline transforms raw public data into a clean analytical dataset.

---

📈 Statistical Modeling

Two advanced statistical frameworks were applied:

1. Mixed Linear Models (MixedLM)
Used to estimate how much of the variation in sales is explained by city‑level differences.

Key result:  
- ICC = 0.6257 → 62.57% of variance is explained at the city level

This means geography is the dominant driver of sales.

2. Generalized Estimating Equations (GEE)
Used to model correlated sales patterns across cities and months.

---

🔍 Key Insights

Seasonality
- December shows a major sales surge  
- October shows a secondary spike  
- January drops sharply after the holiday peak  

Store Density
- Adding one liquor store to a city increases expected sales by ~$26,000 (statistically significant)

City-Level Effects
- City differences explain the majority of sales variation  
- Some cities consistently outperform even after adjusting for store count

Trend
- Long‑term monthly trend is small and statistically non‑significant

---

🎨 Visualizations

This project includes:

- Coefficient impact charts  
- Variance decomposition (ICC) graphics  
- Seasonal trend plots  
- City‑month heatmaps  
- Tableau dashboard (interactive)

These visuals help stakeholders understand complex statistical results quickly.

---

🛠️ Tech Stack

- SQL: DuckDB  
- Python: Pandas, NumPy  
- StatsModels: MixedLM, GEE  
- Visualization: Seaborn, Matplotlib  
- Dashboard: Tableau Public  
- Tools: Jupyter Notebook, GitHub  

---

📁 Repository Structure

`
iowa-liquor-sales/
│
├── data/                # optional sample or schema
├── notebooks/           # full analysis in Jupyter
├── sql/                 # DuckDB SQL scripts
├── visuals/             # charts, ICC graphics, coefficient plots
└── README.md            # project documentation
`

---

🔗 Notebook & Dashboard

- Kaggle Notebook:  
  https://www.kaggle.com/code/shoshanamiriamlevin/iwoa-liquaor-mixlm-by-yaakov-levin (kaggle.com in Bing)

- Tableau Dashboard:  
  

---

📬 Contact

Email: yaylevin99@gmail.com  
Location: Israel  

---

If you want, I can also create:

- A README banner (ASCII or graphic style)  
- A short LinkedIn post announcing the project  
- A GitHub profile README to make your whole account look professional  
- A project thumbnail image you can upload to GitHub  
