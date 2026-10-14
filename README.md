# Wafer CMP Material-Removal-Rate Modelling with Symbolic Regression (PHM 2016)

Chemical-mechanical planarization (CMP) data from the PHM Society 2016 Data Challenge: a full data audit, cleaning, feature engineering and insight study of ~2,800 wafer polishing runs, followed by a resumable PySR symbolic-regression study that looks for interpretable, Preston-like equations for the removal rate under three evaluation protocols.

## Contents

| File | What it does |
|---|---|
| `notebooks/01_preprocessing_eda_insights.ipynb` | PHM 2016 Data Challenge (CMP) — Data Preprocessing, EDA & Insights |
| `notebooks/02_symbolic_regression_study.ipynb` | CMP symbolic regression — complete notebook using Colab versions |

Notebooks are saved with the outputs of their last run, so results and figures can be read on GitHub without running anything.

## Data

PHM Society 2016 Data Challenge (CMP). The notebooks fetch the pinned GitHub mirror `akangel0307/PHM-Data-Challenge`.

## How to run

The notebooks were developed on Google Colab. Upload a notebook to Colab (File → Upload notebook) and run the cells in order; the first cells install anything missing. To run locally in VS Code instead: `python -m venv .venv`, activate it, `pip install -r requirements.txt jupyter`, then open the notebook and pick the `.venv` kernel. Cells that mount Google Drive (`google.colab`) can be skipped locally if the data files are placed next to the notebook. PySR needs Julia; the notebook installs it on first run.

Python packages used: `ipython`, `matplotlib`, `numpy`, `pandas`, `pysr`, `requests`, `scikit-learn`, `scipy`, `seaborn`, `sympy` (see `requirements.txt`).

## License

MIT, see `LICENSE`.
