# Automated ETL Pipeline for Fashion Product Data

## 📖 Overview

This project develops an end-to-end Extract, Transform, Load (ETL) pipeline to automate the collection, cleaning, transformation, and storage of fashion product data from an e-commerce website. The pipeline was built using modular Python code and follows software engineering best practices, including unit testing and error handling.

The extracted data is transformed into an analysis-ready dataset before being stored in multiple data repositories, enabling efficient access for downstream analytics and machine learning tasks.

---

## 🎯 Business Problem

Fashion retailers need up-to-date competitor product information to support pricing strategies, product analysis, and market monitoring. Manually collecting and preparing this data is time-consuming, error-prone, and difficult to maintain as product catalogs continue to grow.

---

## 💡 Solution

This project automates the entire ETL process by scraping product information from a fashion e-commerce website, cleaning and validating the extracted data, transforming it into a structured format, and loading the processed data into multiple storage destinations. The pipeline is implemented using modular code, incorporates error handling, and is validated through automated unit testing.

---

## 📂 Dataset

- **Source:** Fashion Studio (Dicoding ETL Project)
- **Website:** https://fashion-studio.dicoding.dev
- **Data:** Fashion product information
- **Fields:**
  - Product Title
  - Price
  - Rating
  - Colors
  - Size
  - Gender
  - Timestamp

---

## ⚙️ Project Workflow

```text
Fashion Studio Website
        │
        ▼
Data Extraction
(Web Scraping)
        │
        ▼
Data Transformation
(Data Cleaning,
Data Validation,
Currency Conversion,
Type Conversion,
Duplicate Removal)
        │
        ▼
Data Loading
(CSV,
Google Sheets,
PostgreSQL)
        │
        ▼
Unit Testing
(Test Coverage)
```

---

## 📊 Results

- Automated extraction of fashion product data from multiple website pages.
- Cleaned and transformed the scraped dataset through data validation, duplicate removal, missing value handling, and currency conversion.
- Loaded the processed data into **CSV**, **Google Sheets**, and **PostgreSQL** repositories.
- Implemented modular ETL architecture with **unit testing**, **error handling**, and **80–100% test coverage**, achieving a **5-Star (Advanced)** project evaluation in Dicoding.

---

## 📁 Repository Structure

```text
automated-etl-pipeline-fashion-product-data/
│
├── README.md
├── requirements.txt
├── submission.txt
├── main.py
│
├── utils/
│   ├── extract.py
│   ├── transform.py
│   └── load.py
│
├── tests/
│   ├── test_extract.py
│   ├── test_transform.py
│   └── test_load.py
│
├── data/
│   └── products.csv
│
└── credentials/
    └── google-sheets-api.json
```

## 🚀 How to Run

Clone the repository.

```bash
git clone https://github.com/CarmenLisapaly/automated-etl-pipeline-fashion-product-data.git
```

Install dependencies.

```bash
pip install -r requirements.txt
```

Run the ETL pipeline.

```bash
python main.py
```

Run unit tests.

```bash
python -m unittest discover -s tests
```

Generate test coverage.

```bash
coverage run -m unittest discover -s tests
coverage report -m
```

### Url Google Sheets:
https://docs.google.com/spreadsheets/d/1oIxZtCuPFbzuYMxkOWabo4xSjc5FTdrJ5erN122FZY4/edit?usp=sharing
