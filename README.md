# Scikit-Learn-Regression
Diabetes regression analysis using the built-in dataset from Scikit-learn. This project builds and compares three machine learning regression models to predict disease progression. Models are trained, evaluated with metrics like MSE and R^2, and analyzed to determine the best performing approach.

# Project Purpose
The purpose of this project is to explore machine learning regression techniques using Python and the Scikit-learn library. The project uses the built-in diabetes dataset to train and evaluate multiple regression models that predict disease progression based on patient health measurements. By comparing several models, the goal is to determine which regression approach produces the most accurate predictions.

# Project Overview
This program loads the diabetes dataset provided by Scikit-learn, prepares the data for machine learning, and builds several regression models. The dataset is divided into training and testing sets to ensure that models are evaluated on unseen data. Each model is trained using the training dataset and evaluated using statistical performance metrics.

The results are then compared to determine which model performs best at predicting diabetes progression.

# Class Design and Implementation
The project is organized using a class-based structure to improve readability, organization, and reusability. The main class is responsible for loading the dataset, preparing the data, training machine learning models, and evaluating their performance.

Encapsulating the machine learning workflow inside a class makes the program easier to maintain and extend if additional models or datasets are added later.

# Class Attributes
The class includes several attributes used throughout the machine learning process:
- data
Stores the dataset loaded from the Scikit-learn diabetes dataset.
- features (X)
Contains the input variables used to train the models.
- target (y)
Contains the output variable representing diabetes disease progression.
- X_train, X_test
Training and testing feature datasets created after splitting the data.
- y_train, y_test
Training and testing target datasets used for model evaluation.
- models
Stores the machine learning models used in the project.

# Class Methods
- load_data()
This method loads the diabetes dataset from Scikit-learn and converts it into a structured format for analysis.

- split_data()
This method divides the dataset into training and testing sets using a standard train-test split. This ensures that models are evaluated on unseen data.

- train_models()
This method initializes and trains multiple regression models using the training dataset. Each model learns patterns in the data in order to make predictions.

-evaluate_models()
This method tests each trained model using the testing dataset and calculates performance metrics such as Mean Squared Error (MSE) and R² score.

-run()
This method executes the full workflow of the program, including loading the dataset, splitting the data, training models, and evaluating performance.

# Machine Learning Models Used

The following regression models were implemented:
- Linear Regression
- Decision Tree Regression
- Random Forest Regression
Each model was trained and evaluated to compare predictive performance.

# Evaluation Metrics
Model performance was evaluated using:
- Mean Squared Error (MSE) – measures prediction error
- R^2 Score – measures how well the model explains variance in the data
These metrics help determine which model performs best.

# Limitations
Several limitations exist in this project:
- The dataset is relatively small, which may limit model generalization.
- Only a few regression models were tested.
- Hyperparameter tuning was not extensively explored.
- The project focuses on predictive performance rather than interpretability of medical outcomes.
Future improvements could include testing additional models, performing hyperparameter optimization, and applying cross-validation techniques.

# Conclusion
This project demonstrates how machine learning regression models can be used to analyze medical datasets and predict disease progression. By comparing different algorithms, the project highlights how model selection can significantly impact predictive performance.
