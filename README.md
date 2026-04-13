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

1. **Data:** Put ACS table folders and exactly one `PLACES*.csv` under **`raw_data/`** (see the notebook’s *Setup* cell for required folder names). The notebook reads only from `raw_data/` and writes to `processed_data/` and `output/`.
2. **Start Jupyter** (with the venv activated):

   ```bash
   jupyter notebook predoc_assessment_pipeline.ipynb
   ```

   Or use JupyterLab / VS Code / Cursor to open the notebook and run all cells from the top.

**Python:** 3.10+ recommended.
