1. Objective

To design, implement, and evaluate a Deep Neural Network (DNN) using the PyTorch framework. Students will gain hands-on experience in data preprocessing, tensor manipulation, and the construction of a multi-class classification pipeline.

 

2. Problem Statement

The Seeds dataset contains measurements of geometrical properties of kernels belonging to three different varieties of wheat: Kama, Rosa, and Canadian. The goal is to build a predictive model that can accurately classify a seed based on seven numerical attributes.

 

3. Laboratory Requirements & Procedure

 

Task A: Data Ingestion and Exploration

Action: Load the seeds_dataset.txt or .csv using pandas.
Exploration: Identify the seven features (Area, Perimeter, Compactness, Length, Width, Asymmetry Coefficient, Groove Length) and the target label (Variety).
Verification: Check for missing values and visualize class distribution to ensure the dataset is balanced.
 

Task B: Data Pre-processing

Normalization: Since the features have different scales (e.g., Area vs. Compactness), apply StandardScaler or MinMaxScaler. This is critical for the convergence of the neural network.
Label Encoding: Ensure target labels are zero-indexed (0, 1, 2) as required by PyTorch’s CrossEntropyLoss.
 

Task C: Dataset Splitting

Action: Divide the processed data into Training and Testing sets (typically an 80/20 split).
Tool: Use train_test_split from sklearn.model_selection.
 

Task D: Tensor Conversion

Action: Convert the NumPy arrays/Pandas DataFrames into torch.Tensor objects.
Data Types: Ensure features are float32 and labels are long (integers).
