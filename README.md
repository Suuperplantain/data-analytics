# Data Analytics Coursework

A structured data analytics coursework project built in Python and delivered as a Jupyter Notebook. This repository presents an exploratory analysis of a laptop dataset, focusing on pricing, brand diversity, ratings, and display characteristics using core data analysis tools such as Pandas, NumPy, Matplotlib, and Seaborn.

The notebook appears to have been authored and executed in a Kaggle environment, then exported into this repository. The analysis is task-driven and answers a series of coursework questions using real dataset operations rather than placeholder examples.

---

## Project Overview

This project demonstrates a practical workflow for introductory to intermediate data analysis:

- loading structured datasets into Pandas DataFrames
- inspecting and preparing data for analysis
- answering coursework-style business and descriptive analytics questions
- extracting key numerical insights from tabular data
- presenting findings in a reproducible notebook format

Although the notebook imports both a laptop dataset and an insurance dataset, the analysis currently implemented in the notebook is centred on the **laptop dataset**.

---

## What the Notebook Covers

The coursework notebook includes scenario-based tasks around laptop data analysis, including:

### 1. Dataset preparation and ordering
The notebook creates a working DataFrame and sorts laptop entries by rating in descending order. The ratings column is cleaned into a format that is easier to work with numerically.

### 2. Brand diversity analysis
The analysis calculates the number of unique laptop manufacturers in the dataset.

**Result recorded in the notebook:**
- **9 unique brands**

### 3. Highest and lowest priced laptops
The notebook identifies the most expensive and least expensive laptops using the `discount_price` field.

**Results recorded in the notebook:**
- **Highest priced laptop:** MacBook Pro (Retina + Touch Bar) — **12499.0**
- **Lowest priced laptop:** IdeaPad S130-14IGM — **899.0**

### 4. Price distribution analysis
The notebook uses descriptive statistics to understand how laptop prices are distributed across the dataset, including count, mean, standard deviation, quartiles, minimum, and maximum values.

**Discount price summary recorded in the notebook:**
- Count: **205**
- Mean: **3812.55**
- Standard deviation: **2308.70**
- Minimum: **899.0**
- 25th percentile: **2099.0**
- Median: **3149.0**
- 75th percentile: **4939.0**
- Maximum: **12499.0**

**Old price summary recorded in the notebook:**
- Count: **205**
- Mean: **4040.36**
- Standard deviation: **2327.15**
- Minimum: **999.0**
- 25th percentile: **2249.0**
- Median: **3299.0**
- 75th percentile: **5649.0**
- Maximum: **12499.0**

### 5. Display size analysis
The notebook also evaluates laptop screen sizes using minimum, maximum, and average display size values.

**Results recorded in the notebook:**
- **Smallest screen:** 12.0
- **Largest screen:** 17.3
- **Average screen size:** 15.1439

---

## Datasets Used

The notebook references the following datasets:

- `laptops.xlsx`
- `insurance(in).csv`

From the notebook content, the primary analysis in this repository is performed on the **laptop dataset**. The insurance dataset is imported but is not part of the visible completed analysis tasks in the current notebook version.

---

## Technologies and Libraries

This project uses:

- **Python 3**
- **Jupyter Notebook**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**

The notebook metadata indicates it was executed in a **Kaggle Python environment**.

---

## Repository Structure

```text
.
├── README.md
└── data-analytics-coursework.ipynb
```

---

## Key Analytical Techniques Demonstrated

The notebook demonstrates several core data analytics techniques that are useful in coursework, portfolio projects, and early-stage industry analysis work:

- reading Excel and CSV files into DataFrames
- previewing and inspecting tabular data
- cleaning rating values into a more usable format
- sorting records by a selected metric
- counting unique categorical values
- locating rows associated with minimum and maximum values
- generating descriptive statistics with `.describe()`
- calculating summary measures such as mean, min, and max

---

## How to Run the Project

### Option 1: Run in Jupyter locally

1. Make sure Python 3 is installed.
2. Install the required libraries.
3. Open the notebook in Jupyter Notebook or JupyterLab.
4. Update the dataset file paths if you are not using Kaggle.
5. Run the notebook cells in order.

Install the common dependencies with:

```bash
pip install notebook pandas numpy matplotlib seaborn openpyxl
```

Then start Jupyter:

```bash
jupyter notebook
```

---

## Important Note About File Paths

The notebook currently loads data using Kaggle-style paths:

```python
pd.read_excel('/kaggle/input/laptops/laptops.xlsx')
pd.read_csv('/kaggle/input/insurance/insurance(in).csv')
```

If you want to run this project locally, change those paths to match your local file locations. For example:

```python
df = pd.read_excel('data/laptops.xlsx')
ins = pd.read_csv('data/insurance(in).csv')
```

This is important because the notebook, in its current state, expects a Kaggle input directory structure.

---

## Strengths of the Project

This coursework project is strong as a university submission and GitHub portfolio item because it shows:

- clear use of Python for real data analysis
- correct use of Pandas for answering specific analytical questions
- structured, task-based reasoning
- use of descriptive statistics to support conclusions
- notebook-based documentation of both code and written explanation

---

## Areas That Could Be Improved Further

To take this from a solid coursework submission to a stronger portfolio project, the following improvements would make a noticeable difference:

### 1. Add data visualisations
The project imports Matplotlib and Seaborn, but the visible notebook analysis is mostly numerical. Adding visualisations would improve presentation and depth.

Examples:
- price distribution histograms
- brand frequency bar charts
- box plots for discount price vs old price
- scatter plots for display size vs price

### 2. Add a dedicated data cleaning section
A short section that explicitly explains cleaning steps would make the workflow more professional and easier to assess.

### 3. Separate findings from code
A final summary section with key findings and business-style conclusions would improve readability.

### 4. Add reproducible project folders
A more complete project structure could include:

```text
.
├── data/
├── notebooks/
├── outputs/
├── requirements.txt
└── README.md
```

### 5. Add dataset provenance
It would strengthen the repo to mention where the datasets came from and whether they were modified before use.

---

## Suggested Future Extensions

Possible future upgrades for this project include:

- discount percentage analysis
- correlation analysis between price and screen size
- brand-level average price comparison
- identification of best value laptops using rating-to-price ratio
- missing value checks and data quality reporting
- export of cleaned data to CSV for reuse
- dashboard version using Streamlit or Power BI

---

## Academic Context

This repository contains coursework submitted as part of a university data analytics project. It is presented here to document the work, showcase the analysis process, and demonstrate practical Python-based data analysis skills.

---

## Author

**Terkaudoon Abbo**  
BSc Computing & Artificial Intelligence  
Nottingham Trent University

---

## License

University project. All rights reserved.

This repository is provided for academic, assessment, and portfolio purposes only. No permission is granted to copy, redistribute, modify, submit, or commercially use this work without prior written permission from the author.
