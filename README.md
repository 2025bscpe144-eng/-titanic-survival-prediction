# -titanic-survival-prediction
Machine learning classification project predicting Titanic passenger survival using a Random Forest Classifier — built from scratch in Python (Pandas, Scikit-learn) with 76.97% accuracy.
#  Titanic Survival Prediction

A beginner machine learning classification project that predicts whether a passenger 
survived the Titanic disaster, based on features like age, gender, ticket class, and fare.

##  Project Overview

This project walks through a complete end-to-end machine learning workflow: loading 
real-world data, cleaning it, engineering features, training a model, and evaluating 
its performance.

- **Dataset:** Titanic passenger data (891 records)
- **Problem Type:** Binary Classification (Survived: Yes/No)
- **Model Used:** Random Forest Classifier
- **Accuracy Achieved:** 76.97%

##  Dataset Features

| Feature | Description |
|---------|-------------|
| Pclass | Ticket class (1st, 2nd, 3rd) |
| Sex | Passenger gender |
| Age | Passenger age |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Fare | Ticket fare paid |
| Embarked | Port of embarkation (Cherbourg, Queenstown, Southampton) |

##  Workflow

1. **Data Loading** — Imported the Titanic dataset using Pandas
2. **Exploratory Data Analysis (EDA)** — Used `.info()` and `.describe()` to understand 
   data structure and spot missing values
3. **Data Cleaning**
   - Filled missing `Age` values with the median
   - Dropped `Cabin`, `Ticket`, and `Name` (not useful for prediction)
   - Removed remaining rows with missing values
4. **Feature Encoding**
   - Converted `Sex` to numeric (male: 0, female: 1)
   - One-hot encoded `Embarked` into separate binary columns
5. **Train/Test Split** — Split data 80/20 for training and evaluation
6. **Model Training** — Trained a `RandomForestClassifier` on the training set
7. **Evaluation** — Measured accuracy on unseen test data

##  Data Visualization

Explored key patterns before modeling, including:
- Survival rate by gender
- Survival rate by passenger class
- Age distribution of passengers
- Feature correlation heatmap

##  Tools & Libraries

- Python 3
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
- Google Colab (development environment)

##  How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com)
2. Run all cells from top to bottom
3. The dataset loads directly from a public GitHub URL — no manual download needed

##  Key Learnings

- Handling missing data effectively
- Converting categorical variables into model-usable numeric form
- Understanding the difference between classification and regression problems
- Evaluating model performance using accuracy metrics

##  Author

**Daniyal Nawaz**
Computer Engineering Student, UET Lahore (Faisalabad Campus)
[LinkedIn](https://linkedin.com/in/daniyal-nawaz-8a5b80410) | [GitHub](https://github.com/2025bscpe144-eng)

---
*This project is part of my self-taught journey into Data Science and Machine Learning.*
