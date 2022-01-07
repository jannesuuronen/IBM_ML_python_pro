# Final Project for "Machine Learning with Python", a course by the IBM Skills Network

The purpose of this final project is train a set of supervised Machine Learning classifiers and determine which the best using the provided datasets: `loan_train.csv` and `loan_test.csv`, with the ultimate goal to applying what we've learnt in the course. 

## Problem Definition
The two dataset, already split into training and test subsets, describes a set of loan takers/customers that either have not or have paidoff their loans. The target is to predict whether a customer will pay off or have their loan end up collected. The two cases are represented by the `"PAIDOFF"` and `"COLLECTION"` labels. Thus we are working with a binary classification problem. 

The following classifiers are considered in this project:
- K-nearest Neighbours
- Decision Tree
- Support Vector Machine
- Logistic Regression

## Evaluation
We evaluathe model's accuracy using the dataset stored in `loan_test.csv` and three metrics **Jaccard score**, **F1 score** and **LogLoss**(in the case of Logistic Regression). 

### Evaluation Matrix
| Algorithm          | Jaccard | F1-score | LogLoss |
| ------------------ | ------- | -------- | ------- |
| KNN                | 0.6     | 0.75     | NA      |
| Decision Tree      | 0.57    | 0.73     | NA      |
| SVM                | 0.72    | 0.84     | NA      |
| LogisticRegression | 0.74    | 0.85     | 0.56    |

By a narrow margin, **Logistic Regression** is the best performing model based on comparable metrics.
