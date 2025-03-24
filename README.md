# growthLinkTask
A repository of the task given by  GrowthLink for Intern position
This project is a machine learning model that predicts passenger survival on the Titanic based on available dataset features. The dataset is preprocessed, and a RandomForestClassifier is trained and tested for performance.

📌 Features Used for Prediction

Pclass (Passenger class)

Sex (Encoded as 0 = male, 1 = female)

Age (Missing values filled with random values between mean ± standard deviation)

SibSp (Number of siblings/spouses aboard)

Parch (Number of parents/children aboard)

Fare (Ticket fare, standardized)

Deck (Extracted from Cabin, encoded as numerical categories)

Embarked (Encoded as categorical values)

🚀 Steps to Run the Project

Clone the Repository

git clone https://github.com/raghavendrashande/growthLinkTask

Run the Model

python titanicSurvivalPrediction.ipynb

Evaluate Performance

The accuracy score will be displayed after training.

Feature importance can be analyzed to understand the most influential variables.

📉 Why Limit max_depth and n_estimators?

The dataset contains only 320 training samples after preprocessing.

Too many estimators (n_estimators) or deep trees (max_depth) can lead to overfitting, where the model memorizes training data instead of generalizing.

Optimal settings:

max_depth=5: Ensures the trees are not too complex.

n_estimators=25: Keeps ensemble size manageable while maintaining predictive power.

Using cross-validation instead of a single test split helps verify model generalization.

🛠 Future Improvements

Experiment with other classifiers like Logistic Regression and Gradient Boosting.

Implement hyperparameter tuning to optimize model performance.

Use cross-validation to validate the model instead of a single test split.