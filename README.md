# ZCAFE

This repository contains my tract-level predoctoral research assessment pipeline using:

- **ACS 2015–2019 5-year estimates** predictors
- **CDC PLACES 2021** tract-level outcomes
- a **z-scored neighborhood disadvantage index**
- **bivariate OLS regressions** for poor mental health and obesity

The full workflow is implemented in **`predoc_assessment_pipeline.ipynb`**.

## Repository contents

- `predoc_assessment_pipeline.ipynb` — main analysis notebook
- `requirements.txt` — Python dependencies
- `raw_data/` — input data directory created after downloading and unzipping the raw data archive

## Environment setup

From the project root:

```bash
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Data setup

Download [`raw_data.zip`](https://drive.google.com/file/d/1NQ_7cVUzNHQtc8xA53EdZ0tsj8ciXB-f/view?usp=sharing) and unzip it into the project root.

After unzipping, the project should contain a `raw_data/` directory with:
- the ACS source folders/files used in the analysis
- the PLACES CSV file

The notebook reads input files **only** from `raw_data/`.

## Running the analysis

With the virtual environment activated, launch Jupyter:

```bash
jupyter notebook predoc_assessment_pipeline.ipynb
```

Then run all cells from top to bottom.

You can also open the notebook in VS Code, JupyterLab, or another IDE and run all cells in order.

## Reproducibility notes

Running the notebook from start to finish should reproduce:
- the merged tract-level analytic dataset
- the neighborhood disadvantage index
- descriptive statistics for the index
- the main bivariate OLS results
- the leave-one-domain-out robustness results

## Python version

**Python 3.10+** recommended.
