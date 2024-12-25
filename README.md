# Enhancing Voice Pathology Detection with Ensemble Stacking and Machine Learning
A Novel machine learning technique for diagnosing serious voice disorders like hyperfunctional dysphonia, laryngitis, and vox senilis, enhancing patient care and reducing healthcare costs.

Dataaug_Featureextr.ipynb contains the Following code cells:

* Data Augmentation. 
* Feature Extraction using openSMILE.
* Combining all DataFrames into one for Final Dataframe (Prepared_features1.csv)

Prepared_features1.csv is the Final Dataframe after Feature extraction which is used for further training and testing.

Ensemble_Stacking.ipynb contains the Following code cells:

* ML models with deafult hyperparameters
* Hyperparameter search space for each ML model using optuna
* Ensemble stacking, Training all the models and base models are choosed on ranking and meta model is trained on the predictions from the four base models.
* ROC-AUC curve
* Confusion Matrix plot for base models and Meta model
* Classification report for each model.

