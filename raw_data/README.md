# Raw data

The raw ACS/PLACES CSVs are **too large for GitHub’s normal git limits** (100MB/file). This repo tracks only the folder scaffold. To reproduce results, use a `raw_data.zip` bundle uploaded as a **GitHub Release asset**.

## For users (after clone)

1. Download `raw_data.zip` from **Releases**
2. Unzip into the project root so it creates/overwrites `raw_data/`

Example:

```bash
unzip raw_data.zip -d .
```

## For you (creating the zip)

From the project root, create the bundle:

```bash
zip -r raw_data.zip raw_data
shasum -a 256 raw_data.zip > raw_data.zip.sha256
```

The pipeline reads only from `raw_data/`.
