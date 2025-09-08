# LG Aimers Hackerton

This repository collects the notebooks and result files created for the LG Aimers Hackerton sales forecasting competition.  The goal is to predict the next 7 days of menu item demand for each store.  Models are built primarily with **LightGBM** and **XGBoost**, and evaluation is based on a weighted SMAPE metric.

## Repository Structure
- `0811_LGBM/Model_lgbm.ipynb` – LightGBM baseline with holiday features
- `0812_LGBM/Model_lgbm_optuna.ipynb` – LightGBM tuned with Optuna
- `0813_XGBoost/code_xgboost.ipynb` – Initial XGBoost prototype
- `0815_XGBoost/code_xgboost_weighted_2.ipynb` – Weighted XGBoost with additional features
- `0817_XGBoost/code_xgboost_more_features _and_weighted.ipynb` – More features and weighting
- `0819_XGBoost/code_xgboost_weighted_2_weightadd.ipynb` – Weighted XGBoost with added weights
- `0822_XGBoost/code_xgboost_weighted_2_weightadd.ipynb` – Updated weights for XGBoost
- `0824_XGBoost/code_xgboost_weighted_2_weightadd.ipynb` – Final XGBoost adjustments
- `docs.pdf` – Competition report (Korean)
- `LICENSE` – MIT license

## Getting Started
### Prerequisites
- Python 3.9+
- Jupyter Notebook
- Suggested packages:
  ```bash
  pip install pandas numpy lightgbm xgboost scikit-learn optuna joblib
  ```

### Data Preparation
Download the competition dataset and place the following files in the project root:
- `train.csv`
- `sample_submission.csv`
- `TEST_00.csv` … `TEST_09.csv`

### Running a Notebook
1. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
2. Open the notebook of interest (e.g., `0811_LGBM/Model_lgbm.ipynb`).
3. Run all cells to train the model and generate `submission.csv` in the notebook directory.

## License
This project is released under the [MIT License](LICENSE).
