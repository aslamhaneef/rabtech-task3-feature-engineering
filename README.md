# RabTech Academy Task 3 — Feature Engineering & Preprocessing Pipeline

## Deliverable
`03_feature_engineering_pipeline.ipynb`

The notebook is designed to match the Task 3 requirements shown in the assignment:

- load a complex tabular dataset
- use `ColumnTransformer`
- scale numerical variables
- one-hot encode categorical variables
- split train/test before learned transformations
- build reusable scikit-learn pipelines
- engineer features inside the pipeline
- perform tree-based feature importance analysis
- check for target leakage

## Dataset
The notebook uses the **UCI Adult (Census Income)** dataset through the official `ucimlrepo` loader.

Official source:
https://archive.ics.uci.edu/dataset/2/adult

Citation:
Becker, B. & Kohavi, R. (1996). Adult [Dataset]. UCI Machine Learning Repository.
DOI: https://doi.org/10.24432/C5XW20

License: CC BY 4.0 (as listed by UCI).

## How to run
1. Open the notebook in Google Colab, Jupyter Notebook, JupyterLab, or VS Code.
2. If needed, uncomment the `%pip -q install ucimlrepo` cell.
3. Run **all cells from top to bottom**.
4. The notebook downloads the official dataset, fits the preprocessing pipeline on the training split, evaluates the hold-out set, and creates `feature_importance.csv`.

## Important
The notebook intentionally does not claim that the resulting model is production-ready. The dataset contains demographic variables, and feature importance is presented as a technical diagnostic rather than a causal or fairness conclusion.
