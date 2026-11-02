# TP5 – Data Normalisation and Class Balancing

##  Project Overview

This project focuses on two important data preprocessing techniques in Machine Learning:

- **Normalisation and Standardisation**
- **Class Balancing (Oversampling and Undersampling)**

The Titanic dataset is used to apply these techniques and understand how they improve data preparation.

##  Dataset

The project uses the Titanic dataset from GitHub.

- **Dataset:** Titanic
- **Target variable:** `Survived`
- `0` = Did not survive
- `1` = Survived

##  Technologies and Libraries

- Python
- Pandas
- Matplotlib
- Scikit-learn
- Imbalanced-learn
- Google Colab / Jupyter Notebook

##  Part 1: Normalisation and Standardisation

Two scaling techniques are applied to the `Age` and `Fare` features.

### 1. Min-Max Normalisation

Transforms values into a range between 0 and 1.

### 2. Z-score Standardisation

Transforms values so that the mean is approximately 0 and the standard deviation is 1.

**Visualisations:**

![Normalisation and Standardisation](images/normalisation.png)

##  Part 2: Class Balancing

The Titanic dataset contains an imbalance between survivors and non-survivors.

Three techniques are applied:

### 1. Random Undersampling
Reduces the number of examples in the majority class.

![Random Undersampling](images/undersampling.png)

### 2. Random Oversampling
Duplicates examples from the minority class.

![Random Oversampling](images/oversampling.png)

### 3. SMOTE
Creates synthetic examples for the minority class.

![SMOTE](images/smote.png)

##  Results

Before balancing:
- Non-survivors: 549
- Survivors: 342

After Random Undersampling:
- Non-survivors: 342
- Survivors: 342

After Random Oversampling:
- Non-survivors: 549
- Survivors: 549

After SMOTE:
- Non-survivors: 549
- Survivors: 549

##  Conclusion

This project helped me understand the importance of data preprocessing in Machine Learning.

Normalisation and standardisation help put numerical features on comparable scales, while balancing techniques help deal with imbalanced datasets.

Each balancing technique has advantages and disadvantages, so choosing the right one depends on the dataset and the problem.

##  Project Structure

```text
TP5-Normalisation-Balancing/
│
├── images/
│   ├── normalisation.png
│   ├── undersampling.png
│   ├── oversampling.png
│   └── smote.png
│
├── TP5_Normalisation_Balancing.ipynb
└── README.md
```

##  Author

Created as part of a Data Mining course practical assignment.# normalisation-et-balancing
 Normalisation, standardisation et rééquilibrage des classes sur le dataset Titanic avec Python (Google Colab). Application de Min-Max Scaling, Z-score, Undersampling, Oversampling et SMOTE.
