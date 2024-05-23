# Digital VLSI Design: Leakage Prediction of C499 Circuit Using ML
This project aims to leverage machine learning techniques to accurately predict leakage power in CMOS circuits, addressing the challenges posed by conventional testing methods.

## Objectives
1. Dataset Generation: Generate datasets for standard cells across various technology nodes, with a focus on the gates involved in the ISCAS-85 C499 complex circuit. Sampling Process, Voltage, and Temperature (PVT) combinations from predetermined distributions to simulate circuits.

2. Exploratory Data Analysis (EDA): Analyze how leakage and delay vary with technology nodes through comprehensive EDA on the generated dataset.

3. Model Training and Prediction: Train separate models for each standard cell type at the 22nm MGK/HP technology node. Utilize these models to predict leakage power for each standard cell in the C499 circuit and estimate the total leakage power of C499.

## Repository Contents

- Datasets: Contains datasets generated for standard cells at different technology nodes, focusing on the gates involved in the C499 circuit.
- Data Analysis: Includes scripts and notebooks for exploratory data analysis to gain insights into leakage and delay variations across different technology nodes.
- ML Model: Contains trained machine learning models for predicting leakage power in CMOS circuits, specifically tailored for the C499 circuit.
- Docs: Detailed documentation, including methodology, results, and insights obtained from the project.
- Tech Nodes: 7 separate files for 7 different tech nodes, each folder comprising of the netlists, dataset generation scripts, outputs and the EDA scripts. 

## Machine Learning Approaches

Two distinct machine-learning approaches are used to predict leakage power in CMOS circuits: **Meta-Learning and Mathematical Transformations.**

### Meta-Learning:

Approach: **The Reptile algorithm**, a meta-learning technique, is utilized for rapid adaptation to new tasks. It involves initializing model parameters randomly for each task, performing task-specific optimization through gradient descent, and updating model parameters based on observed changes in task-specific parameters. The Reptile algorithm enables fast adaptation to new instances or variations in leakage power prediction tasks. It facilitates efficient training and enhances the model's ability to generalize across tasks, improving prediction accuracy.

### Mathematical Transformations:

Approach: Various mathematical transformations, including PCA, standard scaling, feature engineering, quantile transform, and Yeo Johnson's transformation, are applied to the data to enhance model performance. These transformations aim to normalize feature distributions, capture complex relationships, and improve the interpretability of the models. By transforming features and creating new ones based on domain knowledge, the models can learn complex patterns more effectively. Different transformations are applied to address specific characteristics of the data and improve the models' ability to capture non-linear relationships.
These machine learning approaches, combined with comprehensive dataset generation and exploratory data analysis, contribute to accurate leakage power prediction in CMOS circuits.

## Team Members
- Sri Anvith Dosapati
- Sankalp S Bhat
- Shreeya Singh
- Srujana Vanka
  
--- 
