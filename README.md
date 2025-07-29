#  Credit Risk Prediction

## Introduction
This project implements a credit risk prediction model using a benchmark dataset. The primary goal is to predict whether a borrower will experience serious delinquency within two years. The project uses various machine learning models, including a custom `PerpetualBooster`, and `AutoGluon` for automated machine learning.

## Features
- **Data Analysis:** In-depth exploratory data analysis (EDA) to understand feature distributions and relationships.
- **Feature Engineering:** Creation of new features to improve model performance.
- **Model Training:** Implementation and comparison of multiple models, including Logistic Regression, KNN, SVM, Decision Tree, Random Forest, Gradient Boosting, XGBoost, and LightGBM.
- **Hyperparameter Tuning:** Utilization of Optuna for hyperparameter optimization of the best-performing model.
- **AutoML:** Application of AutoGluon for automated model selection and training.
- **Model Interpretability:** Use of SHAP to explain model predictions.

## Architecture and Workflow
1. **Data Ingestion:** The project starts by loading the "Credit Risk Benchmark Dataset".
2. **Exploratory Data Analysis:** The `01-exploratory-data-analysis.ipynb` notebook performs a thorough EDA, including visualizing feature distributions, checking for outliers, and analyzing correlations.
3. **Feature Engineering:** New features are created, such as `is_income_zero` and `worst_delinquency_status`, to capture more complex patterns in the data.
4. **Prediction Model:** The `02-prediction-model.ipynb` notebook trains and evaluates various machine learning models. It also includes hyperparameter tuning with Optuna and model interpretation with SHAP.
5. **AutoML:** The `03-automl.ipynb` notebook uses AutoGluon to automatically find the best-performing model and `PerpetualBooster` for a custom modeling approach.
6. **Output:** The processed dataset and trained models are saved in the `output` directory.

## Project Structure
```
├── .gitignore
├── LICENSE
├── pdm.lock
├── pyproject.toml
├── readme-instruction.md
├── README.md
├── datasets
│   ├── Credit Risk Benchmark Dataset.csv
│   └── README.md
├── notebooks
│   ├── 01-exploratory-data-analysis.ipynb
│   ├── 02-prediction-model.ipynb
│   └── 03-automl.ipynb
├── output
│   ├── datasets
│   │   └── credit_risk_model_ready.csv
│   └── models
│       ├── AutogluonModels
│       └── perpetual
│           └── perpetual_booster_risk_model.json
└── references
```
- **datasets:** Contains the raw and processed data.
- **notebooks:** Jupyter notebooks for data analysis, model training, and AutoML.
- **output:** Stores the processed dataset and trained models.
- **references:** Contains reference materials.

## Getting Started

### Prerequisites
- Python 3.12
- PDM

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-risk-prediction.git
   cd credit-risk-prediction
   ```
2. Install the dependencies using PDM:
   ```bash
   pdm install
   ```

## Usage
To run the project, you can execute the Jupyter notebooks in the `notebooks` directory.

## Note on Data and Models
The dataset used in this project is publicly available from Kaggle. The trained models are saved in the `output/models` directory. The project is fully reproducible.

## Results and Outputs
The project produces the following outputs:
- A processed, model-ready dataset located at `output/datasets/credit_risk_model_ready.csv`.
- Trained models from AutoGluon and PerpetualBooster, saved in the `output/models` directory.
- The best performing model from the manual and AutoML training process is Gradient Boosting and NeuralNetFastAI, with an F1 score of approximately 0.78.

## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue for any bugs, feature requests, or improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.