# Machine Learning-Based Intrusion Detection System for Minority/Rare-Class Attacks

## A. Project Description

The project aims to develop a machine learning-based Intrusion Detection System to resolve the challenge of detecting minority/rare class attacks. It implements advanced machine learning algorithms, Random Forest and XGBoost, combined with the Synthetic Minority Oversampling Technique (SMOTE). The preprocessing methods include:

- **Baseline Model without SMOTE**: Models trained on the original imbalanced dataset.
- **Downsampling with SMOTE**: The majority classes are downsampled to match minority classes, and SMOTE generates synthetic samples.
- **Customized SMOTE**: Each minority class has at least 5,000 samples while maintaining the majority class sizes.

The focus is on improving precision, recall, and F1-scores for minority/rare classes, making the system suitable for real-world scenarios.

---

## B. Features

### Setting

#### Models
- **Random Forest**: Ensemble learning for robust classification.
- **XGBoost**: Gradient-boosting framework for tabular data.

#### Dataset
- **CICIDS2017**: Wednesday and Thursday morning data.
Wednesday (dataset_1) : https://drive.google.com/file/d/1zOeCqtGZjAj_nSLe3W5MH5pDQM28bPde/view?usp=sharing
Thursday morning (dataset_3) : https://drive.google.com/file/d/1WL00LFkCA2ylV8_8c6jm52bnEhGLcKsq/view?usp=sharing
#### Evaluation Metrics
- **Overall**: Accuracy, Precision, Recall, F1-score, and AUC.
- **Minority Classes**: Precision, Recall, and F1-score.
- **Visualization**: Confusion Matrices, Precision-Recall Bar Chart, ROC Curve, Per-Class Metrics Line Plot.

### Data Preprocessing

#### Common Framework
- Load datasets and analyze class distribution.
- Address class imbalance using SMOTE.
- Scale features to optimize model performance.

#### Distinctive Features
- **Baseline Model**: Trains models without SMOTE.
- **Downsampling with SMOTE**: Balances data by downsampling majority classes and applying SMOTE.
- **Customized SMOTE**: Ensures each minority class has at least 5,000 samples.

### Model Implementation

#### Common Framework
- Standard training with cross-validation and hyperparameter tuning.

#### Distinctive Features
- **Baseline Model**: Highlights biases from imbalanced data.
- **Downsampling with SMOTE**: Emphasizes reduced dataset size.
- **Customized SMOTE**: Maximizes recall for minority classes.

---

## C. Installation

### Prerequisites
- **Programming Language**: Python 3.8 or later.
- **Environment**: Jupyter Notebook or Jupyter Lab.

### Setup and Usage
1. Choose one of the following notebooks:
   - `Xgboost&RandomForest-With_Customized_SMOTE.ipynb`
   - `Xgboost&RandomForest-Without_SMOTE.ipynb`
   - `Xgboost&RandomForest-With_Downsampling_SMOTE.ipynb`
2. Execute cells sequentially:
   - Load datasets and check distributions.
   - Apply chosen preprocessing method.
   - Train Random Forest and XGBoost models.
   - Evaluate results using metrics and visualizations.

### Outputs
- **Performance Report**: Accuracy, Recall, F1-score.
- **Visualization**: Confusion Matrix, Precision-Recall Bar Chart, ROC Curve, Per-Class Metrics Line Plot.
- **Comparative Analysis Report**: Preprocessing methods results.

---

## D. Results

### Overall Model Performance
| Preprocessing Method    | Random Forest - Accuracy | XGBoost - Accuracy |
|--------------------------|--------------------------|---------------------|
| Without SMOTE (Baseline) | 0.9985                  | 0.9989             |
| Downsampling + SMOTE     | 0.9979                  | 0.9984             |
| Customized SMOTE         | 0.9984                  | 0.9987             |

### Minority/Rare Classes Results
| Preprocessing Method    | Minority Class | Precision | Recall | F1-Score |
|--------------------------|----------------|-----------|--------|----------|
| Without SMOTE (Baseline) | XSS            | 0.45      | 0.11   | 0.18     |
| Downsampling + SMOTE     | XSS            | 0.42      | 0.67   | 0.51     |
| Customized SMOTE         | XSS            | 0.45      | 0.69   | 0.55     |

---

## E. Credits 

### Collaboration of Project
- **Team members**: Yoojin Jung, Meena Ruwandi, Siwon Lim
- Special thanks to Prof.Zhida Li for leading us by expert guidance, insightful feedback, and unwavering support, which were instrumental in the successful completion of this project.



### Tools and libraries 
- [Scikit-learn](https://scikit-learn.org/stable/)





