# Dynamic ML Pipeline

This repository contains a Jupyter Notebook implementation of a dynamic machine learning pipeline. The notebook parses a JSON configuration file to automate tasks such as feature handling, reduction, model building, and hyperparameter tuning.

---

## Features
- **JSON Parsing**: Reads configuration files to set up the ML pipeline.
- **Feature Engineering**: Handles missing values, scaling, and transformations.
- **Feature Reduction**: Supports PCA, Tree-Based, and Correlation-based techniques.
- **Model Selection**: Dynamically selects models based on the configuration.
- **Hyperparameter Tuning**: Implements GridSearchCV for parameter optimization.
- **Metrics Evaluation**: Outputs R2 Score, Mean Absolute Error, and RMSE.

---

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/dynamic_ml_pipeline.git
    cd dynamic_ml_pipeline
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

---

## Usage
1. Open the Jupyter Notebook:
    ```bash
    jupyter notebook Test.ipynb
    ```
2. Ensure the following files are in the project directory:
    - JSON Configuration File (e.g., `algoparams_from_ui.json`)
    - Dataset File (e.g., `iris.csv`)
3. Follow the steps in the notebook to execute the pipeline.

---

## Example JSON Configuration
```json
{
    "session_name": "test",
    "session_description": "test",
    "design_state_data": {
        "target": {
            "prediction_type": "Regression",
            "target": "petal_width"
        },
        ...
    }
}
