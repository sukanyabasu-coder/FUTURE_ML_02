# FUTURE_ML_02
# Support Ticket Classification System

## Overview

This project is an NLP-based Support Ticket Classification System developed as part of the Future Interns Machine Learning Internship (Task 2).

The system automatically:

* Classifies support tickets into categories
* Assigns ticket priority levels
* Helps automate support workflow management

The project uses Natural Language Processing (NLP) and Machine Learning techniques to improve ticket handling efficiency.

---

## Features

* Text preprocessing and cleaning
* TF-IDF Vectorization
* Multi-class ticket classification
* Priority assignment (High / Medium / Low)
* Interactive ticket prediction system
* Model evaluation and comparison
* Confusion matrix visualization
* Business-oriented workflow automation

---

## Technologies Used

* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Dataset

The dataset contains support tickets with:

* Ticket text (`Document`)
* Ticket category (`Topic_group`)

Categories include:

* Access
* Hardware
* HR Support
* Storage
* Purchase
* Administrative rights
* Miscellaneous
* Internal Project

---

## Machine Learning Workflow

1. Dataset Loading
2. Exploratory Data Analysis
3. Text Understanding
4. Feature and Label Separation
5. Train-Test Split
6. TF-IDF Vectorization
7. Baseline Model Training (Naive Bayes)
8. Model Evaluation
9. Class Imbalance Analysis
10. Balanced Logistic Regression
11. Priority Mapping Logic
12. Interactive Ticket Prediction
13. Visualization and Analysis

---

## Models Used

### 1. Multinomial Naive Bayes

Used as the baseline NLP classifier.

### 2. Logistic Regression (Balanced)

Implemented using:

```python
class_weight='balanced'
```

This improved:

* overall accuracy
* minority class recall
* prediction fairness

---

## Model Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Naive Bayes         | 73%      |
| Logistic Regression | 84%      |

The balanced Logistic Regression model significantly improved the overall system performance.

---

## Priority Assignment Logic

| Category              | Priority |
| --------------------- | -------- |
| Access                | High     |
| Administrative rights | High     |
| Hardware              | High     |
| HR Support            | Medium   |
| Internal Project      | Medium   |
| Storage               | Medium   |
| Miscellaneous         | Low      |
| Purchase              | Low      |

---

## Example Prediction

### Input

```text
Unable to login to office VPN
```

### Output

```text
Predicted Category: Access
Predicted Priority: High
```

---

## Visualizations Included

* Ticket category distribution
* Model accuracy comparison
* Priority distribution
* Confusion matrix

---

## Key Learnings

* NLP preprocessing techniques
* TF-IDF Vectorization
* Text Classification
* Handling Class Imbalance
* Model Evaluation and Comparison
* Business Rule Integration
* Interactive Prediction Systems

---

## Conclusion

This project successfully demonstrates an end-to-end NLP-based support ticket classification pipeline. The balanced Logistic Regression model achieved strong performance and provided more reliable predictions across categories. The system also integrates business-oriented priority assignment to simulate a practical support automation workflow.

---

## Internship Information

Future Interns — Machine Learning Internship (Task 2)
