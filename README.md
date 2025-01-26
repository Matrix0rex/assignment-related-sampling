# assignment-related-sampling

The dataset contains anonymized transaction features, along with a Class column indicating:

0: Legitimate transaction
1: Fraudulent transaction
The dataset is highly imbalanced, with fraudulent transactions constituting only a small percentage of the total.


Project Steps
1. Data Preprocessing
Loaded the dataset (Creditcard_data.csv) and analyzed its structure.
Checked for missing values and handled any necessary cleaning.
Scaled the features using techniques like MinMaxScaler (if required) to ensure compatibility with models.
2. Sampling Techniques
To address the class imbalance, five sampling methods were applied:

Sample 1: Simple Random Sampling (SRS)
A random subset of the dataset was selected without focusing on class proportions.
Sample 2: Stratified Sampling
Ensured that both classes (0 and 1) were represented in the same proportion as the original dataset.
Sample 3: Systematic Sampling
Selected every n-th transaction from the dataset.
Sample 4: Oversampling (Best Performing Sample)
Increased the number of minority class (Class=1) instances using techniques like SMOTE (Synthetic Minority Oversampling Technique) to create a balanced dataset.
Outcome: This method achieved the highest accuracy across multiple models.
Sample 5: Undersampling
Reduced the majority class (Class=0) instances to match the size of the minority class, achieving balance by sacrificing some data.
3. Model Training and Evaluation
The following models were applied to each sample:

Random Forest
Logistic Regression
Support Vector Machine (SVM)
K-Nearest Neighbors (KNN)
Decision Tree
Evaluation Metric: Accuracy was used as the primary metric to compare model performance on each sample.

