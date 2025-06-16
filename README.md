# Insurance Risk Analytics Project

## Project Overview

This project analyzes historical car insurance claim data for AlphaCare Insurance Solutions (ACIS) to optimize marketing strategy and identify low-risk targets for premium reduction. The analysis spans from February 2014 to August 2015 and includes various features about policies, clients, vehicles, and claims.

## Project Structure

insurance-risk-analytics/
├── data/ # Raw and processed data (DVC tracked)
├── notebooks/ # Jupyter notebooks for EDA and analysis
├── src/ # Source code (data, eda, features, models, utils)
├── tests/ # Unit tests
├── outputs/ # Plots, metrics, and reports
├── .github/ # GitHub Actions workflows
├── .dvc/ # DVC metadata
├── README.md
├── dvc.yaml
├── environment.yml
├── requirements.txt

## Setup Instructions

1. **Clone the repository:**

   ```bash
   git clone [repository-url]
   cd insurance-risk-analytics
   ```

2. **Create and activate the environment:**

   ```bash
   conda env create -f environment.yml
   conda activate insurance-risk-analytics
   ```

3. **Install DVC (if not already installed):**

   ```bash
   pip install dvc
   ```

4. **Pull the data from DVC remote:**
   ```bash
   dvc pull
   ```

## Data Version Control (DVC)

- The project uses DVC to track and version data files.
- Data is **not stored in Git**; only small `.dvc` pointer files are.
- To add new data or update, use:
  ```bash
  dvc add data/raw/your_file.csv
  git add data/raw/your_file.csv.dvc .dvc/config .dvcignore
  git commit -m "Add new data version"
  dvc push
  ```

## Project Tasks & Progress

### Task 1: EDA & Statistics (✅ Completed)

- Data understanding and quality assessment
- Exploratory Data Analysis (EDA) with summary statistics, distributions, outlier detection, and visualizations
- Key findings summarized for data quality, geographic, and vehicle risk patterns

### Task 2: Data Version Control (✅ Completed)

- DVC initialized and configured with a local remote
- Data tracked and versioned with DVC
- Data pipeline is reproducible and auditable

### Task 3: Hypothesis Testing (Next)

- Risk differences across provinces, zip codes, and genders
- Margin differences between zip codes

### Task 4: Predictive Modeling (Next)

- Claim severity prediction
- Premium optimization
- Model interpretation and feature importance

## How to Reproduce

1. Clone the repo and set up the environment as above.
2. Run `dvc pull` to get the data.
3. Open and run the notebooks in the `notebooks/` directory for EDA and further analysis.
