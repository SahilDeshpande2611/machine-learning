# Heart Disease Prediction

A machine learning project to predict the presence of heart disease using clinical and demographic data.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training & Evaluation](#model-training--evaluation)
- [Exported Models](#exported-models)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project demonstrates a complete workflow for heart disease prediction, including:
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Feature engineering and encoding
- Model training and evaluation with multiple algorithms
- Saving trained models for deployment

## Project Structure

```
Heart_Disease_pred/
│
├── heart.csv                # Dataset file (not included)
├── heart_disease.ipynb      # Main Jupyter notebook
├── KNN_heart.pkl            # Saved KNN model
├── scaler.pkl               # Saved scaler
├── columns.pkl              # Feature columns used for training
├── README.md                # Project documentation
└── requirements.txt         # (Optional) Python dependencies
```

## Dataset

- The dataset (`heart.csv`) should be placed in the project directory.
- It contains clinical and demographic features relevant to heart disease.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd Heart_Disease_pred
    ```

2. (Optional) Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
    If `requirements.txt` is not present, install these packages:
    ```bash
    pip install numpy pandas matplotlib seaborn scikit-learn joblib
    ```

## Usage

1. Launch Jupyter Notebook:
    ```bash
    jupyter notebook heart_disease.ipynb
    ```

2. Follow the notebook cells for:
    - Data loading and inspection
    - Data cleaning and preprocessing
    - Exploratory data analysis (EDA)
    - Model training and evaluation

3. The notebook saves the best model and preprocessing objects for future use.

## Model Training & Evaluation

- Models used: Logistic Regression, K-Nearest Neighbors (KNN), Naive Bayes, Decision Tree, Support Vector Machine (SVM)
- Evaluation metrics: Accuracy, F1-score, Classification report
- The best-performing model is saved as `KNN_heart.pkl`.

## Exported Models

- `KNN_heart.pkl`: Trained KNN model
- `scaler.pkl`: StandardScaler object used for feature scaling
- `columns.pkl`: List of feature columns used for training

These files can be used for deployment or inference on new data.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.
