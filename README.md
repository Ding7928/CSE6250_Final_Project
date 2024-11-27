Reproducibility of Ensemble Methods for Record Linkage
Overview
This repository implements and evaluates ensemble methods (Bagging and Stacking) for record linkage tasks using both real and synthetic datasets. It demonstrates the effectiveness of ensemble methods compared to basic learners (SVM, Logistic Regression, and Neural Network).
Dependencies
The following packages are required to run the code:

Python (version 3.8 or higher)
pandas
numpy
scikit-learn
xgboost
recordlinkage
matplotlib
To install these dependencies, use:


Copy code
pip install pandas numpy scikit-learn xgboost recordlinkage matplotlib
Datasets
Real Dataset: ePBRN dataset (ensure you have legal access and save the file as .csv).
Synthetic Dataset: FEBRL dataset (generated using FEBRL's official generator).
No pretrained models are required as all models are trained from scratch.

Functionality of Scripts
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


Copy code
git https://github.com/mchen920329/CSE6250_Final_Project

Place the Datasets

Add your .csv datasets to the data/ directory.
Set Up the Working Directory
In your script, specify the working directory as follows:

python
Copy code
import os
os.chdir('/path/to/your/project')
Run Preprocessing
Prepare the datasets for training and testing:


Copy code
python preprocess_data.py
Train and Evaluate Models
Train basic learners and ensemble methods, and evaluate their performance:


Copy code
python train_and_evaluate.py
Visualizations
Results (e.g., bar charts and confusion matrices) will be saved in the results/ directory.

Example Output
Bar Charts: Comparing the performance of basic learners and ensemble methods.
Confusion Matrices: Highlighting true positives, true negatives, false positives, and false negatives for all models.
