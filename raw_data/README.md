# Raw data

Place **exactly one** PLACES tract CSV matching `PLACES*.csv` and the **seven** ACS 2019 5-year table folders here, using the same names the Census download uses (see the notebook *Setup* cell, `ACS_FOLDER_NAMES`).

You can symlink from elsewhere on disk or copy the folders into this directory. The pipeline reads only from `raw_data/` and never from duplicate copies at the repository root.
