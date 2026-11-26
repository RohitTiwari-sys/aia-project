# Breast Cancer Diagnosis Prediction (AIA Project)

Machine learning project that predicts whether a breast tumour is **malignant or benign** from cell-nucleus measurements (Breast Cancer Wisconsin Diagnostic dataset).

## Project structure
```
.
├── Breast_Cancer_Prediction_AIA_Project.ipynb   # full workflow with outputs
├── data/data.csv                                # dataset
├── svm_breast_cancer_model.joblib               # trained model
├── requirements.txt
└── README.md
```

## Workflow
1. Load dataset
2. Model selection (5 models compared with 5-fold cross-validation)
3. Cleaning: missing values, duplicates, label encoding, correlation analysis, removal of redundant features
4. Stratified 80/20 train-test split
5. Training and hyperparameter tuning (SVM with GridSearchCV)
6. Evaluation: accuracy, precision, recall, F1, ROC-AUC, confusion matrix, ROC curve, feature importance

## Result (test set)
Accuracy 97.4% | Precision 100% | Recall 92.9% | F1 96.3% | ROC-AUC 0.995

## Run locally
```
pip install -r requirements.txt
jupyter notebook Breast_Cancer_Prediction_AIA_Project.ipynb
```

## Dataset
Breast Cancer Wisconsin (Diagnostic) Data Set, available on Kaggle and the UCI ML Repository.

*Educational project, not a clinical diagnostic tool.*
