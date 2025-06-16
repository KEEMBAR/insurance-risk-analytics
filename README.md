# Insurance Risk Analytics Project

## Project Overview

This project analyzes historical car insurance claim data for AlphaCare Insurance Solutions (ACIS) to optimize marketing strategy and identify low-risk targets for premium reduction. The analysis spans from February 2014 to August 2015 and includes various features about policies, clients, vehicles, and claims.

## Project Structure

```
insurance-risk-analytics/
├── data/                      # Raw and processed data tracked by DVC
├── notebooks/                 # Jupyter notebooks for analysis
├── src/                       # Source code
├── tests/                     # Unit tests
├── outputs/                   # Outputs like plots and reports
└── docs/                      # Documentation
```

## Setup Instructions

1. Clone the repository:

```bash
git clone [repository-url]
cd insurance-risk-analytics
```

2. Create and activate the conda environment:

```bash
conda env create -f environment.yml
conda activate insurance-risk-analytics
```

3. Initialize DVC:

```bash
dvc init
```

## Project Tasks

### Task 1: EDA & Statistics

- Data understanding and quality assessment
- Exploratory Data Analysis
- Statistical analysis of key metrics

### Task 2: Data Version Control

- DVC setup and configuration
- Data pipeline implementation

### Task 3: Hypothesis Testing

- Risk differences across provinces
- Risk differences between zip codes
- Margin differences between zip codes
- Risk differences between genders

### Task 4: Predictive Modeling

- Claim severity prediction
- Premium optimization
- Model interpretation and feature importance
