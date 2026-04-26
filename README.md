
# 10 Academy: Artificial Intelligence Mastery

## Week 0 Challenge — African Climate Trend Analysis

---

## Overview

This project is part of the Week 0 challenge for the 10 Academy AI Mastery program. The objective is to establish a solid development workflow and perform exploratory data analysis (EDA) on African climate datasets in preparation for deeper analysis related to COP32.

---

## Project Objectives

### Task 1: Git & Environment Setup

* Set up a Git-based workflow using best practices.
* Configure a Python development environment.
* Implement Continuous Integration (CI) using GitHub Actions.
* Document setup and reproducibility steps.

### Task 2: Data Profiling, Cleaning & EDA

* Clean and preprocess climate datasets.
* Perform exploratory data analysis (EDA) per country.
* Extract insights on temperature, rainfall, and related variables.

---

## Repository Structure

```
├── .vscode/
│   └── settings.json
├── .github/
│   └── workflows/
│       └── ci.yml
├── .gitignore
├── requirements.txt
├── README.md
├── src/
├── notebooks/
│   ├── __init__.py
│   └── README.md
├── tests/
│   └── __init__.py
└── scripts/
    ├── __init__.py
    └── README.md
```

---

## Environment Setup

### 1. Clone Repository

```bash
git clone https://github.com/<your-username>/climate-challenge-week0.git
cd climate-challenge-week0
```

### 2. Create Virtual Environment

Using `venv`:

```bash
python -m venv venv
source venv/bin/activate      # Linux/Mac
venv\Scripts\activate         # Windows
```

Or using `conda`:

```bash
conda create -n climate-env python=3.x
conda activate climate-env
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Git Workflow

* Create a setup branch:

```bash
git checkout -b setup-task
```

* Follow Conventional Commits:

  * `init: add .gitignore`
  * `chore: setup virtual environment`
  * `ci: add GitHub Actions workflow`

* Open a Pull Request and merge into `main`.

---

## Continuous Integration

A GitHub Actions workflow is configured to run on every push to `main`.
It performs:

* Python environment check or
* Dependency installation via `requirements.txt`

File location:

```
.github/workflows/ci.yml
```

---

## Data Processing & EDA

### Branch Naming

```
eda-<country>
```

Example:

```
eda-ethiopia
```

### Notebook Naming

```
<country>_eda.ipynb
```

---

## Data Cleaning Steps

* Replace `-999` values with `NaN` (NASA missing value indicator).
* Remove duplicate rows and document findings.
* Convert `YEAR` and `DOY` into a proper datetime column.
* Extract `Month` for seasonal analysis.
* Handle missing values:

  * Forward-fill weather variables or
  * Drop rows with >30% missing values

---

## Analysis Performed

### 1. Summary Statistics

* Descriptive statistics (`df.describe()`)
* Missing value analysis (`df.isna().sum()`)

### 2. Outlier Detection

* Z-score method (|Z| > 3)
* Document decision: drop, cap, or retain

### 3. Time Series Analysis

* Monthly average temperature (T2M)
* Monthly precipitation totals (PRECTOTCORR)
* Identification of seasonal patterns

### 4. Correlation Analysis

* Correlation heatmap
* Key relationships:

  * T2M vs RH2M
  * T2M_RANGE vs WS2M

### 5. Distribution Analysis

* Histogram of precipitation
* Bubble chart: temperature vs humidity with rainfall


---