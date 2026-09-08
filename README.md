# Sudoku
Sudoku Puzzle


# Overview

This project demonstrates a machine learning approach for Sudoku completion using an incomplete Sudoku puzzle as input.

# Dataset

The dataset contains 1,000,000 Sudoku puzzles with:

* `quizzes` – incomplete Sudoku puzzles represented as 81-digit strings
* `solutions` – corresponding completed Sudoku solutions represented as 81-digit strings

A sample of the dataset was used for model training and experimentation.

# Approach

1. Loaded and explored the Sudoku dataset.
2. Checked for missing values and duplicate records.
3. Converted the Sudoku puzzle into 81 numerical features.
4. Used the solution digit as the target variable.
5. Split the data into training and testing sets.
6. Trained a Random Forest Classifier.
7. Evaluated the model using accuracy, classification report, and 5-fold cross-validation.
8. Saved the trained model using Joblib.

# Model

*Random Forest Classifier*

The current implementation demonstrates Sudoku digit prediction as the machine learning component of Sudoku completion.

# Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Joblib
* Jupyter Notebook

# Files

* `Sudoku_Model.ipynb` – Notebook containing data processing, model training, prediction, and evaluation.
* `sudoku_model.pkl` – Saved trained Random Forest model.

# Future Enhancement

The current implementation predicts a Sudoku digit as a proof of concept. The next enhancement would be to extend the model to predict all required cells and combine the predictions with Sudoku constraints to generate a fully completed valid Sudoku grid.
