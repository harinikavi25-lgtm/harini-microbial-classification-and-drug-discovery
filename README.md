# Microbial Classification and Antimicrobial Activity Prediction

## Project Overview
This project combines deep learning and machine learning for:
1. Image-based classification of 33 microbial classes.
2. Computational prediction of antimicrobial activity against Escherichia coli.

## Technologies
- Python
- TensorFlow and Keras
- MobileNetV2
- Random Forest Regression
- Scikit-learn
- Pandas, NumPy and Matplotlib
- ChEMBL database

## Module 1: Microbial Classification

MobileNetV2 transfer learning was used to classify 33 microbial classes.

Test results:
- Accuracy: 83.66%
- Loss: 0.6014
- Macro F1-score: 0.83
- Weighted F1-score: 0.84

## Module 2: Antimicrobial Activity Prediction

A Random Forest regression model was developed using ChEMBL data to predict MIC values against Escherichia coli.

Features:
- Molecular weight
- ALogP
- Hydrogen bond acceptors
- Hydrogen bond donors
- Polar surface area
- Rotatable bonds

Results:
- R2 score: 0.4935
- MAE: 0.5149
- RMSE: 0.877
- Spearman correlation: 0.7412
- Top-10 overlap: 4 compounds

These are preliminary computational results, not experimentally confirmed drug discoveries.

## Dataset

The microbial image dataset contains 2,034 images across 33 classes and is not included in this repository.

The antimicrobial dataset was prepared from the first 1,000 retrieved ChEMBL MIC activity records.

ChEMBL: https://www.ebi.ac.uk/chembl/

## Installation

Install dependencies:

    pip install -r requirements.txt

Launch Jupyter:

    jupyter notebook

Open notebooks/Microbiology_AI.ipynb and configure the image dataset path.

## Limitations
- Performance varies between microbial classes.
- The drug prediction model uses a relatively small dataset.
- Random splitting may place similar compounds in training and testing sets.
- Predicted MIC values require experimental validation.
- This is an academic research prototype, not a clinical diagnostic or drug-development tool.

## Future Scope
- Expand microbial image datasets.
- Improve class-wise classification performance.
- Use larger antimicrobial activity datasets.
- Validate predictions using independent compounds.

## Author
Harini K. R.

B.Tech Biotechnology  
Periyar Maniammai Institute of Science and Technology

## Acknowledgements
ChEMBL, TensorFlow, Keras and Scikit-learn.
