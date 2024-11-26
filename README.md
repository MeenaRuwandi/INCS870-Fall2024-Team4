# **Experiment 5: Experiment With Optimizing SMOTE Ratios**
## **Source Code**
SMOTE-Custom-2-RF_XGBoost.ipynb

## **System Requirements**
1. **Python**: Version 3.9 or higher.
2. **Libraries**:
   - `imbalanced-learn`
   - `scikit-learn`
   - `pandas`
   - `matplotlib`
   - `gdown`
3. **Datasets**:
   - `dataset_1(Wednesday)`: https://drive.google.com/file/d/1zOeCqtGZjAj_nSLe3W5MH5pDQM28bPde/view?usp=sharing
   - `dataset_3(Thursday_Morning)`:
https://drive.google.com/file/d/1WL00LFkCA2ylV8_8c6jm52bnEhGLcKsq/view?usp=sharing					

---

## **Usage**

### **Step 1: Setup & Data Loading and Validation**
Ensure the dataset files are available at the paths specified in the notebook. Update the variable `dataset_paths` if needed:
```python
dataset_paths = [
    '../dataset_1.csv',
    '../dataset_3.csv',
]
```

### **Step 2: Preprocessing**
Includes steps like:
1. Handling missing values.
2. Applying SMOTE to balance the dataset.

### **Step 3: SMOTE & Model Training**
- Train a **Random Forest** and an **XGBoost** model using the balanced dataset.
- Perform hyperparameter tuning if applicable.

### **Step 4: Evaluation**
- Evaluate the models using standard metrics such as accuracy, precision, recall, and F1-score.

---

## **Troubleshooting**
- **File not found**: Verify that all specified datasets exist in the correct path.
- **Library not installed**: Install missing dependencies using `pip install <library-name>`.
- **Memory errors**: Reduce dataset size or use a machine with higher memory capacity.

---

## **Comment**
I sincerely appreciate Professor Zhida and my teammates, Meena and Yoojin, for their support and collaboration.

Siwon Lim<br>
1331833