# TP N°5 – Normalisation and Balancing

##  Project Overview

This project focuses on two important data preprocessing techniques in Machine Learning: **data scaling** and **class balancing**.

Using the Titanic dataset, I applied different techniques to understand how data can be prepared before training a Machine Learning model.

##  Objectives

- Understand the difference between normalisation and standardisation.
- Apply Min-Max Scaling and Z-score Standardisation.
- Understand class imbalance.
- Apply Random Undersampling, Random Oversampling, and SMOTE.
- Compare the results using visualisations.

##  Tools and Libraries

- Python
- Pandas
- Matplotlib
- Scikit-learn
- Imbalanced-learn
- Jupyter Notebook / Google Colab

##  Dataset

The project uses the Titanic dataset.

**Source:** [Titanic Dataset – GitHub](https://github.com/datasciencedojo/datasets/blob/master/titanic.csv)

The target variable is `Survived`:

- `0` – Non-survivors
- `1` – Survivors

## 1. Data Normalisation and Standardisation

In this part, I worked with the `Age` and `Fare` columns.

### Min-Max Normalisation

This technique transforms values into a range between 0 and 1.

### Z-score Standardisation

This technique transforms values so that their mean is approximately 0 and their standard deviation is 1.

Missing values were replaced with the median before applying the transformations.

**Results:**

![Normalisation and Standardisation](images/normalisation-standardisation.jpeg)

## 2. Class Balancing

The original dataset contains more non-survivors than survivors. This creates an imbalance between the two classes.

### Original Distribution

- Non-survivors: 549
- Survivors: 342

![Original Class Distribution](images/before-balancing.jpeg)

### Random Undersampling

This method reduces the majority class by randomly removing some examples.

After undersampling:
- Non-survivors: 342
- Survivors: 342

![Random Undersampling](images/undersampling.jpeg)

### Random Oversampling

This method increases the minority class by randomly duplicating existing examples.

After oversampling:
- Non-survivors: 549
- Survivors: 549

![Random Oversampling](images/oversampling.jpeg)

### SMOTE

SMOTE creates new synthetic examples for the minority class using neighbouring observations.

After SMOTE:
- Non-survivors: 549
- Survivors: 549

![SMOTE](images/smote.jpeg)

## 3. Results Comparison

| Method | Non-survivors (0) | Survivors (1) |
|---|---:|---:|
| Before balancing | 549 | 342 |
| Random Undersampling | 342 | 342 |
| Random Oversampling | 549 | 549 |
| SMOTE | 549 | 549 |

## 4. Conclusion

Through this practical work, I learned how to prepare data using normalisation and standardisation.

I also learned how to handle imbalanced datasets using different techniques.

Random Undersampling removes examples from the majority class, Random Oversampling duplicates examples from the minority class, while SMOTE creates synthetic examples.

These techniques are important because good data preparation can help improve Machine Learning models.

##  Project Structure

```text
normalisation-et-balancing/
│
├── images/
│   ├── normalisation-standardisation.jpeg
│   ├── balancing-comparison.jpeg
│   ├── before-balancing.jpeg
│   ├── undersampling.jpeg
│   ├── oversampling.jpeg
│   └── smote.jpeg
│
├── TP5_Normalisation_Balancing.ipynb
└── README.md
```

##  Author

Created as part of a Data Mining practical assignment.
