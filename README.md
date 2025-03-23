# Enhancing Voice Pathology Detection with Ensemble Stacking and Machine Learning
A Novel machine learning technique for diagnosing serious voice disorders like hyperfunctional dysphonia, laryngitis, and vox senilis, enhancing patient care and reducing healthcare costs.

* Voice disorders affect 5-10% of the population, significantly impairing communication and often leading to social isolation, anxiety, or depression.
* Common conditions like hyperfunctional dysphonia, laryngitis, and vox senilis are frequently observed in neurological disorders, further impacting quality of life.
* These widespread issues also bring substantial costs to individuals and healthcare systems, highlighting the importance of efficient diagnostic tools to improve accuracy and reduce the burden on healthcare services.

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

To evaluate model performance, metrics like accuracy, precision, recall, and F1 score were calculated, with hyperparameters fine-tuned using the Optuna library. This significantly improved the efficiency of all models. Among the base models, KNN achieved the highest accuracy of 89.5%, followed by LS and ETC with 86% and the ensemble model achieving an accuracy of 91.5%. 

* Among the individual classifiers, KNN achieved the highest accuracy of 89%, while ensemble stacking further boosted accuracy to 91%. Looking ahead, future research will focus on expanding the dataset to include more voice disorders and exploring advanced algorithms like deep reinforcement learning, transfer learning, and attention mechanisms to enhance the model’s performance and robustness.


# Cite

Consider citing the Work at
https://doi.org/10.1109/ICMACC62921.2024.10894115
