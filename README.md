# sars-bcell-epitope-prediction
Machine learning pipeline for predicting B-cell epitopes in SARS and COVID-19 proteins, including exploratory data analysis with visualisations, feature engineering, model training, and performance evaluation.

# Disclaimer
This project is created purely for **learning and demonstration purposes**.  
It is **not intended for clinical, medical, or research use**, and the author is **not responsible** for any misuse of this code or its outputs.

# Introduction
B-cell epitopes are regions of antigens recognised by antibodies and are critical for vaccine development. Accurate prediction of these epitopes can guide immunological research and accelerate vaccine design, particularly for emerging viruses like SARS and COVID-19. By leveraging machine learning, researchers can reduce the time required for experimental design in wet lab processes, using computational predictions to prioritise experiments. These predictions can then be validated in the lab, increasing speed and efficiency during urgent health crises. The project applies both feature-based (isoelectric point, hydrophobicity, aromaticity, stability) and heuristic-based (Chou-Fasman β-turn probability, Emini surface accessibility, Kolaskar-Tongaonkar antigenicity, Parker hydrophilicity) engineering to improve model accuracy and ROC-AUC, combining this with model evaluation and exploratory data analysis. **It is intended purely as a learning exercise** to apply bioinformatics and machine learning skills in a practical context.

# Overview
This repository demonstrates a complete workflow for B-cell epitope prediction:
- Loading and cleaning datasets related to SARS and COVID-19 proteins  
- Generating peptide features from IEDB B-cell data  
- Exploratory data analysis including histograms, boxplots, scatter plots, and confusion matrices  
- Training multiple machine learning models (Random Forest, Decision Tree, Logistic Regression)  
- Evaluating models with metrics such as ROC-AUC and visualisations  

The project showcases **bioinformatics, machine learning, and data analysis skills** in a hands-on educational context **only**.

# How to run
1. Open the notebook 'COVID19_Prediction.ipynb' using Jupyter Notebook.
2. Download the datasets (available on Kaggle; https://www.kaggle.com/datasets/futurecorporation/epitope-prediction).
3. Run all cells to reproduce the analysis, trained models, and visualisations.
4. A prompt will open requesting to paste the protein sequence, once pasted, hit enter, to get output (target, epitope (1), or non-epitope (0)).

# Datasets
- Original datasets used for training the model were downloaded from Kaggle.(https://www.kaggle.com/datasets/futurecorporation/epitope-prediction).
- Derived dataset 'peptide_features.csv' was generated from IEDB Analysis Resource (http://www.tools.iedb.org/bcell/help/).
