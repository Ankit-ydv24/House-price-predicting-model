# House Price Predicting Model

A simple, end-to-end machine learning workflow for predicting house prices from tabular data. This project is organized around a Jupyter/Colab notebook (`AI_Project.ipynb`) that walks through data exploration, feature engineering, model training, and evaluation.

## What’s inside

- `AI_Project.ipynb` – the main notebook with all steps:
	- Data loading and basic EDA
	- Preprocessing (handling missing values, encoding categoricals, scaling numerics)
	- Model training (baseline models and improvements)
	- Evaluation (RMSE/MAE/R²) and quick error analysis

## Quick start

### Option A: Open in Google Colab

1. Upload the notebook to Colab or open directly from GitHub.
2. If your dataset is on your local machine, upload it in the Colab session or mount Google Drive.
3. Run all cells. The notebook installs its own Python packages when needed.

### Option B: Run locally (Windows/PowerShell)

```powershell
# Create and activate a virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# Install Jupyter and common packages (adjust as needed)
pip install jupyter numpy pandas scikit-learn matplotlib seaborn

# Launch Jupyter
jupyter notebook
```

Open `AI_Project.ipynb` and run cells top-to-bottom. If your dataset path differs, update the corresponding cell.

## Data

Use a tabular CSV with typical housing features (e.g., area, bedrooms, bathrooms, location). The notebook includes guidance for:

- Handling missing values and outliers
- Encoding categorical columns
- Train/validation split

You can replace the dataset path to point to your CSV and re-run the cells.

## Modeling approach

- Baseline: Linear Regression and Decision Tree
- Improved: Random Forest or Gradient Boosting (e.g., XGBoost/LightGBM if added)
- Preprocessing: StandardScaler for numeric features; OneHotEncoder for categoricals
- Metrics: RMSE, MAE, and R²

Feel free to extend with hyperparameter tuning (GridSearchCV/RandomizedSearchCV) and cross-validation.

## Results

The notebook prints evaluation metrics and plots feature importances for tree-based models. Use these to compare models and iterate.

## Reproducibility tips

- Set random_state for deterministic splits and model training.
- Keep a requirements list if you add new packages:

```txt
numpy
pandas
scikit-learn
matplotlib
seaborn
```

## License

Add a LICENSE file if you plan to reuse or distribute this work.

## Acknowledgements

Built as part of a learning project to practice practical ML on structured data.