> D.A.T.A. WAVE SUMMIT – PHILIPPINE JUNIOR DATA SCIENCE CHALLENGE (HACKATHON) FINANCIAL INCLUSION PROJECT

# Philippine Junior Data Science Challenge 2 — Exploratory Data Analysis

## Project summary

This repository contains an exploratory data analysis (EDA) for the **Philippine Junior Data Science Challenge 2**. The primary work is in the `eda.ipynb` notebook which walks through data loading, cleaning, exploratory visualizations, and answers a set of business questions about customers and credit card transactions.

---

## Table of contents

- [Project summary](#project-summary)
- [Notebook & files](#notebook--files)
- [Data description](#data-description)
- [Analysis pipeline](#analysis-pipeline)
- [Key questions we answer](#key-questions-we-answer)
- [Key findings (summary)](#key-findings-summary)
- [Visualizations](#visualizations-placeholders)
- [How to run](#how-to-run)
- [Project structure](#project-structure)
- [Contributing](#contributing)
- [License](#license--contact)

---

## Notebook & files

- Main notebook: `eda.ipynb` (open in Jupyter / VS Code / GitHub)
- Data: `data/` (place your CSVs or cleaned files here)
- Image assets: `images/` — this folder will contain exported figures referenced below.

---

## Data description

> **Fill in these values from the executed notebook results**

- **Raw files used:** `data/customers.csv`, `data/transactions.csv` (adjust filenames as needed)
- **Number of rows (customers):** `__REPLACE_WITH_NUMBER__`
- **Number of rows (transactions):** `__REPLACE_WITH_NUMBER__`
- **Time-span covered by transactions:** `__REPLACE_WITH_DATES__`
- **Important columns (example):** `customer_id`, `age`, `gender`, `region`, `transaction_id`, `amount`, `merchant`, `txn_date`, `txn_type`.

---

## Analysis pipeline

The notebook follows a canonical EDA pipeline:

1. **Import libraries** — pandas, numpy, matplotlib, seaborn, etc.
2. **Load data** — read CSVs / source files and inspect `df.head()` and `df.info()`.
3. **Data cleaning**
   - Remove duplicates
   - Detect and impute / remove nulls
   - Remove unnecessary columns
   - Convert types (dates, categoricals, numeric)
   - Detect and treat outliers
4. **Feature engineering**
   - Create derived features such as `txn_month`, `avg_amount_per_customer`, `total_spend`, `days_active`.
5. **Exploratory visualizations**
   - Time series of transaction volume and value
   - Distribution of transaction amounts
   - Top merchants and merchant categories
   - Customer segmentation / cohort analysis
   - Correlation matrix and heatmap
6. **Answer business questions & summary** — collect insights and suggested next steps.

---

## Key Fidings

These are the business / analytic questions present in the notebook — update the answers with the notebook outputs:

- Which customer segments have the highest average spend? → `__ANSWER_PLACEHOLDER__`
- How does transaction volume vary over time (seasonality, spikes)? → `__ANSWER_PLACEHOLDER__`
- Which merchants / categories drive the most revenue? → `__ANSWER_PLACEHOLDER__`
- Are there notable outliers or suspicious transactions? → `__ANSWER_PLACEHOLDER__`
- How complete / clean is the dataset (missing data summary)? → `__ANSWER_PLACEHOLDER__`

---

## Key findings (summary)

> Insert the notebook's numeric summary results here. Example format:

- **Total unique customers:** `__REPLACE__`
- **Total transactions:** `__REPLACE__`
- **Median transaction amount:** `__REPLACE__`
- **Top 3 merchant categories by revenue:** `__REPLACE__`
- **Most common transaction day / month:** `__REPLACE__`
- **Data quality issues discovered:** `__REPLACE__` (e.g., columns with high null rates, inconsistent date formats)

---

## Visualizations (placeholders)

Below are recommended images produced by the notebook. Replace the placeholder images in `images/` with the exported figures from your executed notebook and keep the filenames below so the README displays them automatically.

1. Missing values heatmap

```
![Missing values heatmap](images/fig_01_missing_values.png)
```

2. Transaction volume over time (daily/monthly)

```
![Transactions over time](images/fig_02_transactions_over_time.png)
```

3. Distribution of transaction amounts (histogram / boxplot)

```
![Amount distribution](images/fig_03_amount_distribution.png)
```

4. Top merchants by revenue (bar chart)

```
![Top merchants](images/fig_04_top_merchants.png)
```

5. Correlation matrix / heatmap

```
![Correlation matrix](images/fig_05_correlation_matrix.png)
```

6. Customer segmentation scatter / cluster plot

```
![Customer segments](images/fig_06_customer_segments.png)
```

7. Any maps (if customers have region/location)

```
![Geographic distribution](images/fig_07_geo_distribution.png)
```

> Tip: Export each Matplotlib / Seaborn figure from the notebook using `fig.savefig('images/fig_01_missing_values.png', bbox_inches='tight', dpi=150)` so filenames match the placeholders above.

---

## How to run

```bash
# create virtualenv (recommended)
python -m venv venv
source venv/bin/activate   # or `venv\Scripts\activate` on Windows
pip install -r requirements.txt

# open notebook
jupyter lab eda.ipynb
# or
jupyter notebook eda.ipynb
```

If you want to regenerate figures programmatically, run the notebook end-to-end (Kernel -> Restart & Run All) and then export `images/` as shown above.

---

## Project structure

```
├─ README.md
├─ eda.ipynb
├─ requirements.txt
├─ data/
│  ├─ customers.csv
│  └─ transactions.csv
└─ images/
   ├─ fig_01_missing_values.png
   ├─ fig_02_transactions_over_time.png
   └─ ...
```

---

# Authors
- [Mariano, Isaiah John](https://github.com/ice-leo)
- Montealto, Meluisa
- [Regalario, Jeremiah Daniel](https://github.com/jeremiahdanielregalario)

---

## License

This project is licensed under the MIT License 
