                                                              Project Title

                                                              
                              Machine Learning-Based Intrusion Detection System for Minority/Rare-Class Attacks
                              
A. Project Description

The project aims to develop a machine learning-based Intrusion Detection System to resolve the challenge of detecting minority/rare class attacks. It implements advanced classifiers machine learning algorithms, Random Forest and XGBoost, combined with state-of-the-art data balancing method, SMOTE (Synthetic Minority Oversampling Technique). To provide a balanced dataset for Random Forest and XGBoost, SMOTE was applied in two different ways. Besides, as a baseline to compare them, one experiment was conducted without SMOTE.
1)	Baseline Model without SMOTE
For comparison purpose, Random Forest and XGBoost are trained on the original imbalance dataset.
2)	Downsampling with SMOTE
To create a more properly balanced dataset for better performance of both models, two approaches were applied. By utilizing RUS the majority classes are downsampled to match the optimal rate of the minority/rare classes, followed by employing SMOTE to generate synthetic samples for the minority/rare classes. This two-step approach provides a more balanced dataset while maintaining the overall class distribution.
3)	Customized SMOTE
To provide a sufficient dataset for minority/rare classes and keep the data size manageable, a customized SMOTE generates synthetic samples so that each class has at least 5,000 samples for improved performance of both models.
The project focuses on improving precision, recall, and F1 scores for minority/rare classes by discovering and providing an effective machine learning-based intrusion detection system appropriate for real-world scenarios.

B. Features
1.	Setting
   
i) Models
Random Forest and XGBoost are selected to utilize the machine learning model.

ii)	Datasets
CICIDS2017 (Wednesday and Thursday morning)
iii)	Evaluation Metrics
- Evaluation metrics for overall results
 Accuracy, Precision, Recall, F1-score, and AUC

- Evaluation metrics for minority/rare classes
Precision, Recall, and F1-score

- Visualization metrics
Confusion Matrices, Precision-Recall Bar Chart, ROC Curves, Per-Class Metrics Line Plot, Per-Class Metrics Line Plot

2)	Data Preprocessing 
1.	Common Framework in Data Preprocessing 
i)	Loading dataset and analyzing distribution
ii)	Addressing class imbalance using different preprocessing approaches (SMOTE methods).
iii)	Scaling features to optimize the model
2.	Distinctive Features for Each Experimental Method
i)	Baseline Model Without SMOTE
The preprocessing applying SMOTE is not used. The original imbalanced dataset is used to train the models.
ii)	Downsampling with SMOTE
The majority classes are downsampled to match the optimal rate of the minority classes. SMOTE is employed to generate synthetic samples for minority classes, reaching a well-balanced dataset.
iii)	Customized SMOTE
SMOTE oversamples classes under 5000 counts to 5000 counts to balance each class to contain at least 5000 counts. The majority class sizes are maintained, focusing on increasing the representation of minority classes.
2)	Model Implementation
1.	Common Framework in Model Implementation
i)	Random Forest and XGBoost are trained by standard training procedures.
ii)	Robust evaluation is ensured by cross-validation and hyperparameter tuning.
2.	Distinctive Features for Each Experimental Method
i)	Baseline Model Without SMOTE
Random Forest and XGBoost are trained to emphasize the bias generated by the imbalanced dataset. Evaluation metrics reveal the limitations of traditional training procedures without balancing the dataset.
iii)	Downsampling with SMOTE
Both models are modified to function with smaller datasets. Hyperparameter tuning highlights reducing overfitting caused by the reduced size of the majority class.
iv)	Customized SMOTE
Both models are adjusted for balanced datasets, with hyperparameter tuning focusing on maximizing the recall of the minority classes. Model training is enhanced by a consistent class distribution.

C. Installation
1)	Prerequisites
1-1.	Programming Language 
Pyton 3.8 or later
2.	Interactive Environment
Jupyter Notebook or Jupyter Lab
2-1. Setup
3) Usage
3-1. Launch Jupyter Notebook
3-2. Select notebook based on the selecting preprocessing method (SMOTE method) from the list below and open it.
3. Execute the cells sequentially
i) Examine class distributions after loading datsets
ii) Preprocess the dataset utilizing the chosen balancing methods
iii) Train Random Forest and XGBoost
iv) Evaluate results with metrics and visulization
4) Outputs
1.	Model Performance Report: Accuracy, Recall, F1-score
2.	Visualizations Report: 
Confusion Matrix, Precision-Recall Bar Chart, ROC, Curve, 
Per-Class Metrics Line Plot
3.	Comparative analysis report for the preprocessing methods

D. Results



