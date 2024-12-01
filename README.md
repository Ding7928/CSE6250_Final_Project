# Reproducibility of Ensemble Methods for Record Linkage

## Overview

This repository implements and evaluates ensemble methods (Bagging and Stacking) for record linkage tasks using both real and synthetic datasets. It demonstrates the effectiveness of ensemble methods compared to basic learners (SVM, Logistic Regression, and Neural Network).

## Dependencise

**Note:make sure you're in `/CSE50_FINAL_PROJECT` directory**

```sh
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Dataset

**Real Dataset**: ePBRN dataset (ensure you have legal access and save the file as .csv).  
**Synthetic Dataset**: FEBRL dataset (generated using FEBRL's official generator).

<br>
No pretrained models are required as all models are trained from scratch.

## Functionality of Scripts

1. Preprocessing
   Extracts feature vectors based on similarity scores (e.g., given_name, surname, and postcode).
   Implements blocking for candidate pair generation.
   Outputs feature vectors for training and testing.
2. Training
   Implements basic learners: SVM, Logistic Regression, and Neural Network.
   Implements ensemble methods: Bagging and Stacking.
3. Evaluation
   Evaluates models using metrics: Precision, Recall, Accuracy, and F1-score.
   Generates bar charts and confusion matrices to visualize performance.
   Instructions to Run the Code
   Clone the Repository

**Reproduce results for FERBL dataset by running `FERBL.ipynb`**  
**Reproduce results for ePBRN dataset by running `ePBRN.ipynb`**
