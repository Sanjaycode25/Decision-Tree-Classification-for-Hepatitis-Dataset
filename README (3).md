
# Decision Tree Classification for Hepatitis Dataset

This project demonstrates the application of Decision Tree Classifiers to predict the presence of Hepatitis based on various health-related features from a dataset. Two different criteria, Gini Index and Entropy, are used to evaluate and build the decision tree models. The aim is to classify whether a patient has Hepatitis (binary classification).



## Dataset

The dataset used in this project is the Hepatitis Dataset. It includes multiple features, such as demographic information, symptoms, and various blood test results, and it is used to predict the presence of Hepatitis. The target variable is Class, where:

- Class = 1 indicates the presence of Hepatitis,
- Class = 2 indicates the absence of Hepatitis.
## Features:

- Age: The age of the patient.
- Sex: The gender of the patient (binary).
- Steroid: Whether the patient used steroids (binary).
- Antivirals: Whether the patient used antivirals (binary).
- Fatigue: Whether the patient experienced fatigue (binary).
- Malaise: Whether the patient experienced malaise (binary).
- Anorexia: Whether the patient experienced anorexia (binary).
- Liver Big: Whether the liver is enlarged (binary).
- Liver Firm: Whether the liver is firm (binary).
- Spleen Palpable: Whether the spleen is palpable (binary).
- Spiders: Whether spider angiomas are present (binary).
- Ascites: Whether the patient has ascites (binary).
- Varices: Whether varices are present (binary).
- Bilirubin: Bilirubin levels (numeric).
- Alk Phosphate: Alkaline phosphatase levels (numeric).
- Sgot: SGOT (serum glutamic-oxaloacetic transaminase) levels (numeric).
- Albumin: Albumin levels (numeric).
- Protime: Prothrombin time (numeric).
- Histology: Whether the histology of the liver suggests disease (binary).
## Libraries Used

The following Python libraries were used in this project:

- pandas: Used for data manipulation and analysis.
- numpy: Used for numerical operations.
- matplotlib: Used for visualizations, particularly for plotting decision trees.
- seaborn: Used for statistical data visualization.
- scikit-learn: Used for machine learning, including model training, splitting the dataset, and generating evaluation metrics.
- category_encoders: Used for encoding categorical features.
- warnings: Used to suppress unnecessary warnings during the execution.
## Worksteps

- *1.Data Loading and Preprocessing:*
The dataset is read using pandas.read_csv(). Missing values are handled by filling them with the mean of the respective columns. The target variable (Class) is separated from the features, and the data is split into training and testing sets using train_test_split().

- *2.Model Training: Two Decision Tree Classifiers are created:*

Gini Index Classifier: A decision tree classifier that uses the Gini index as the criterion for splitting nodes.
Entropy Classifier: A decision tree classifier that uses entropy (information gain) as the criterion for splitting nodes

- *3.Model Evaluation: Both models are evaluated by:*

- Accuracy: The accuracy of both models is calculated on both the training and test sets.
- Overfitting/Underfitting: The training and test set scores are compared to check for overfitting or underfitting.
- Confusion Matrix: A confusion matrix is generated to visualize the classification results (true positives, false positives, true negatives, false negatives).
- Classification Report: A detailed classification report is generated, which includes precision, recall, F1-score, and support for each class.

- *4.Model Visualization:*
The decision trees for both the Gini and Entropy classifiers are visualized using plot_tree(), which displays the structure of each tree, including splits based on the features and criteria used.
## Results

After running the code, you will obtain the following results:

- Model Accuracy: The accuracy of both the Gini and Entropy classifiers will be displayed for both the training and testing sets. You can compare the performance of the two models.

- Confusion Matrix: The confusion matrix will show the number of true positive, false positive, true negative, and false negative results for each model.

- Classification Report: A classification report will show the precision, recall, F1-score, and support for both classes (Hepatitis and non-Hepatitis).
## Source

Web - UCI Machine Learning Repository

Dataset Name - Hepatitis

Link - https://archive.ics.uci.edu/dataset/46/hepatitis
## License

This project is licensed under the MIT License.