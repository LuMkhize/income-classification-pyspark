# Income Classification with PySpark

This project demonstrates a machine learning pipeline using **Apache Spark (PySpark)** to classify income levels based on demographic data.

## 📄 Dataset

**Source**: [UCI Machine Learning Repository - Adult Data Set](https://archive.ics.uci.edu/ml/datasets/adult)

## 💡 Objective

Predict whether a person earns more than \$50K/year based on features like education, workclass, occupation, etc.

## ⚙️ Technologies Used

- Apache Spark (PySpark)
- Python
- Spark MLlib
- Pandas, NumPy (for auxiliary data inspection)

## 🧪 Pipeline Steps

1. **Data Loading and Cleaning**
   - Read CSV
   - Drop missing values

2. **Feature Engineering**
   - Categorical encoding using `StringIndexer`
   - Feature vector assembly with `VectorAssembler`

3. **Modeling**
   - Trained `RandomForestClassifier` and `DecisionTreeClassifier`
   - Evaluated using Accuracy, Precision, Recall, F1 Score, Confusion Matrix

4. **Evaluation**
   - Used `MulticlassClassificationEvaluator` and `MulticlassMetrics` from Spark ML

## 📊 Results

Both models were evaluated on test data. The results included:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

