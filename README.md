# YoungDevInterns_Artificial-Intelligence-Machine_Learning_AI_Task_6-ML_Task_4
Train a Model with Cross-Validation  Task: Evaluate model performance using cross-validation.  Details:  Implement k-fold cross-validation with a model of your choice.  Assess performance metrics like accuracy, precision, and recall

📌 Task Objective
Build and evaluate a classification model using K-Fold Cross-Validation to assess the consistency and reliability of the model across different data splits.

📊 Dataset
File: preprocessed_cereal.csv

Target: rating_class (derived from rating values categorized into Low, Medium, and High)

⚙️ Methodology
✅ Step-by-Step Breakdown
Preprocessing

Converted numerical rating column into 3 categories using pd.cut()

Encoded target classes using LabelEncoder

Model Selection

Logistic Regression (LogisticRegression(max_iter=1000))

Cross-Validation

Used StratifiedKFold with n_splits=3 to ensure class balance across folds

Evaluation Metrics

Accuracy

Precision (macro average)

Recall (macro average)

F1-score (macro average)

All metrics were calculated using make_scorer and passed into cross_validate.

