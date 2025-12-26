# Biomedical Machine Learning: Classification and Model Comparison

## Project Overview
This project applies machine learning techniques to a biomedical classification dataset.
The objective is to analyze biomedical features, train predictive models, optimize their performance, and compare results using appropriate evaluation metrics.

Support Vector Machine (SVM) and Random Forest classifiers are implemented and evaluated within a structured machine learning pipeline.

---

## Dataset Description
The dataset consists of multiple numerical features derived from biomedical signals.
Each sample is associated with a binary class label representing two physiological or diagnostic conditions.

- **Target variable**: `class` (binary classification)
- **Features**: Numerical biomedical signal features
- **Identifiers**: Non-informative identifiers were removed during preprocessing

---

## Methodology

### 1. Data Understanding and Exploration
- Dataset structure and dimensions were examined.
- Mean values of features were computed.
- Class distribution was analyzed.
- Correlation analysis was performed to understand feature relationships.

### 2. Feature Analysis and Selection
- A correlation heatmap was used to visualize relationships among features.
- Correlation-based feature selection was applied using the target variable.
- Features with stronger relationships to the target were retained.

### 3. Data Preprocessing
- Non-informative columns were removed.
- Missing values were checked and handled if present.
- Features and target variables were separated.
- Feature scaling was applied where required.

### 4. Model Training
Two machine learning models were trained:
- Support Vector Machine (SVM)
- Random Forest

Baseline performance was evaluated using accuracy, confusion matrices, and classification reports.

### 5. Hyperparameter Optimization
- Bayesian Optimization was applied to tune model hyperparameters.
- Cross-validation was used to select optimal configurations.
- Optimized models were retrained and evaluated.

### 6. Model Evaluation and Comparison
- Models were evaluated using:
  - Accuracy
  - Sensitivity (Recall)
  - Specificity
  - F1-score
- Confusion matrices were visualized.
- Comparative performance plots were generated.
- Results were summarized in a tabular format.

### 7. Model Saving
- The tuned SVM and Random Forest models were saved using `joblib` for future deployment or analysis.

---

## Technologies Used
- Python
- NumPy
- Pandas
- Scikit-learn
- Scikit-optimize (Bayesian Optimization)
- Matplotlib
- Seaborn
- Joblib

---

## How to Run the Project
1. Clone the repository.
2. Install required dependencies (see `requirements.txt`).
3. Open the Jupyter Notebook.
4. Run all cells sequentially to reproduce the results.

---

## Results
The final results demonstrate the comparative performance of SVM and Random Forest models on the biomedical dataset.
Visualizations and tables provide insights into classification accuracy and error patterns.

---

## Conclusion
This project demonstrates a complete biomedical machine learning workflow, from data analysis and feature selection to model optimization and evaluation.
The structured approach ensures reliable, interpretable, and reproducible results suitable for biomedical information processing tasks.