# 🌍 GDP, Population & Happiness: A Data Wrangling Case Study

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

## 📌 Overview

This project explores the **relationship between national economic indicators (GDP, population) and happiness scores** across countries worldwide. It demonstrates a complete **end-to-end data wrangling pipeline** — from raw data collection to cleaned analysis-ready datasets and insightful visualizations.

Built as a professional data wrangling case study, this project showcases real-world skills in **data gathering, quality assessment, cleaning, storage, and exploratory data analysis (EDA)**.

---

## ❓ Research Question

**How do GDP and population size relate to a country's happiness score?**

Do wealthier or more populous nations report higher levels of happiness, or is the relationship more nuanced than conventional wisdom suggests?

---

## 📊 Datasets

| Dataset | Source | Gathering Method | Records |
|---------|--------|-----------------|---------|
| **World Happiness Report** | [Kaggle](https://www.kaggle.com/) | Manual Download | 500+ |
| **World Population Data** | GitHub / Wikipedia | Programmatic Download / Web Scraping | 500+ |

Both datasets share **country name** as a common key, enabling a meaningful merge for cross-analysis.

---

## 🛠️ Tech Stack

- **Python 3.8+** — Core programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **Matplotlib & Seaborn** — Data visualization
- **BeautifulSoup4** — Web scraping
- **Requests** — HTTP requests for programmatic data downloads
- **Jupyter Notebook** — Interactive development environment

---

## 📁 Project Structure

```
├── README.md                  # Project documentation
├── requirements.txt           # Python dependencies
├── data_wrangling.ipynb       # Main Jupyter Notebook (full pipeline)
├── raw_happiness_data.csv     # Raw happiness dataset
├── raw_population_data.csv    # Raw population dataset
└── cleaned_merged_data.csv    # Final cleaned and merged dataset
```

---

## 🔄 Data Wrangling Pipeline

### 1. Data Gathering
- **Happiness Data**: Downloaded from Kaggle containing happiness scores, GDP per capita, and other well-being indicators by country.
- **Population Data**: Gathered programmatically using Python (`requests` and `BeautifulSoup`) to collect population statistics by country.

### 2. Data Assessment
Identified and documented **4 data issues** across both datasets:

| #  | Type    | Issue Description |
|----|---------|-------------------|
| 1  | Quality | Missing values in key numerical columns |
| 2  | Quality | Inconsistent country name formatting across datasets |
| 3  | Tidiness | Observational units spread across multiple tables (datasets need merging) |
| 4  | Tidiness | Structural issues requiring reshaping for analysis |

### 3. Data Cleaning
- Handled missing values with appropriate imputation or removal strategies
- Standardized country names for consistent merging
- Merged datasets on country as the common key
- Removed unnecessary variables, retaining 4+ analysis-ready columns
- Validated each cleaning step visually and programmatically

### 4. Data Storage
- Maintained **raw** and **cleaned** versions of all datasets
- Used descriptive file naming conventions for reproducibility

### 5. Exploratory Data Analysis (EDA)
- Produced multiple visualizations to explore relationships between GDP, population, and happiness
- Identified key patterns and insights supported by descriptive statistics

---

## 📈 Key Findings

- Countries with **higher GDP per capita** tend to report **higher happiness scores**, but the relationship shows diminishing returns at higher income levels.
- **Population size alone** is not a strong predictor of national happiness.
- The interplay between economic wealth and happiness is **multifaceted**, suggesting that factors beyond GDP contribute significantly to well-being.

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/gdp-happiness-data-wrangling.git
cd gdp-happiness-data-wrangling

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook data_wrangling.ipynb
```

---

## 🔮 Future Work

- Incorporate additional datasets such as education index, healthcare spending, or inequality metrics (Gini coefficient)
- Perform time-series analysis to track how happiness scores evolve alongside GDP growth
- Apply statistical modeling or machine learning to quantify predictor importance
- Explore regional and continental trends in happiness beyond country-level analysis

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- [World Happiness Report](https://worldhappiness.report/) for the happiness dataset
- [Kaggle](https://www.kaggle.com/) for hosting open datasets
- Udacity Data Science program for project framework and guidance

---

### 📬 Connect

If you found this project interesting or have questions, feel free to reach out or star ⭐ the repository!

---

> *"Data is the new oil, but like oil, it must be refined to be useful."*

**Tags**: `data-wrangling` `python` `pandas` `data-analysis` `eda` `data-cleaning` `jupyter-notebook` `gdp` `happiness-index` `world-population` `data-science` `web-scraping` `beautifulsoup` `data-visualization` `matplotlib` `seaborn`