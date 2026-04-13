# ZCAFE

Tract-level predoc assessment pipeline: ACS 2019 (5-year) variables, PLACES 2021 outcomes, z-scored neighborhood disadvantage index, and OLS regressions. The workflow lives in **`predoc_assessment_pipeline.ipynb`**.

## Environment (virtualenv)

From the project root:

```bash
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Running

1. **Data (required):** Download `raw_data.zip` from Google Drive: `https://drive.google.com/file/d/1NQ_7cVUzNHQtc8xA53EdZ0tsj8ciXB-f/view?usp=sharing` and unzip it into the project root so it creates a `raw_data/` directory (ACS folders + the `PLACES*.csv`). The notebook reads only from `raw_data/`.
2. **Start Jupyter** (with the venv activated):

   ```bash
   jupyter notebook predoc_assessment_pipeline.ipynb
   ```

   Or use any IDE to open the notebook and run all cells from the top.

**Python:** 3.10+ recommended.
