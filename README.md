# Student Performance Analysis and Prediction

## Project Overview

This project explores student performance using Exploratory Data Analysis (EDA), data preprocessing, visualization, and a deep learning classification model. A TensorFlow/Keras Multilayer Perceptron (MLP) predicts one of three performance categories—Low, Average, or High—from student demographic, family, school, and study-habit features.

## Objectives

- Analyze student information using statistical summaries and visualizations.
- Identify patterns and relationships among selected student attributes.
- Handle missing values, duplicates, categorical variables, and numerical feature scaling.
- Develop a deep learning model for three-class student performance classification.
- Evaluate the model using appropriate classification metrics and visualizations.

## Dataset

**Source:** UCI Machine Learning Repository — Student Performance

https://archive.ics.uci.edu/dataset/320/student%2Bperformance

This project uses the mathematics dataset (`student-mat.csv`). The original mathematics dataset contains 395 student records and 33 columns.

The target variable `Performance` is derived from the final grade `G3` using these project-defined thresholds:

- **Low:** G3 below 10
- **Average:** G3 from 10 through 14
- **High:** G3 from 15 through 20

`G1`, `G2`, and `G3` are excluded from model input features to avoid target leakage.

## Technologies Used

- Python
- Google Colab / Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- TensorFlow and Keras

## Project Workflow

1. Dataset acquisition and inspection
2. Exploratory data analysis
3. Data cleaning and preprocessing
4. Feature encoding and scaling
5. Training, validation, and test split
6. MLP model development and validation-based hyperparameter selection
7. Final test-set evaluation
8. Visualization, reporting, and result export

## Evaluation

The final model is evaluated using:

- Accuracy and balanced accuracy
- Macro precision, recall, and F1-score
- Weighted F1-score
- Confusion matrix
- One-vs-rest ROC curves and AUC, where supported by the test data

**Final test results**

| Metric | Result |
|---|---|
| Test accuracy | Replace with measured result |
| Balanced accuracy | Replace with measured result |
| Macro precision | Replace with measured result |
| Macro recall | Replace with measured result |
| Macro F1-score | Replace with measured result |
| Macro ROC-AUC | Replace with measured result, if available |

## Repository Structure

```text
Student-Performance-Analysis/
├── Student_Performance_Analysis.ipynb
├── README.md
├── requirements.txt
├── evaluation_results/
├── visualizations/
├── models/
└── Report.pdf
```

Some files or folders may be absent if they have not been generated or if the optional report has not yet been added.

## How to Run

1. Open `Student_Performance_Analysis.ipynb` in Google Colab.
2. Run the notebook cells in order.
3. The notebook downloads the dataset from the UCI repository.
4. Install any missing dependencies listed in `requirements.txt`.
5. Run the preprocessing, model training, and evaluation sections to generate the results.

The notebook is the primary source for the complete workflow.

## Limitations

- The mathematics dataset is relatively small.
- Model performance may vary across different student populations.
- The three performance categories are defined for this project and are not official labels supplied by UCI.
- Predictions are estimates and should not be treated as definitive judgments about individual students.

## Future Enhancements

- Validate the model on additional student datasets.
- Compare the MLP with traditional machine learning classifiers.
- Improve interpretability using feature-importance or explainability techniques.
- Develop a simple interface for demonstration and prediction.

## References

1. Cortez, P., & Silva, A. (2008). *Using data mining to predict secondary school student performance*. [Add the verified publication link or DOI after checking the source.]
2. UCI Machine Learning Repository. *Student Performance*. https://archive.ics.uci.edu/dataset/320/student%2Bperformance
3. TensorFlow. *Keras documentation*. https://www.tensorflow.org/guide/keras
4. Scikit-learn. *Model evaluation documentation*. https://scikit-learn.org/stable/modules/model_evaluation.html
