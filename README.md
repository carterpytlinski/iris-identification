# Iris Flower Classification with K-Nearest Neighbors (KNN)

## Project Overview

This project demonstrates classification of Iris flowers using the K-Nearest Neighbors (KNN) algorithm.

The Iris dataset contains 150 flowers across 3 species:
• Setosa
• Versicolor
• Virginica

Each flower has 4 features: 1. Sepal length (cm) 2. Sepal width (cm) 3. Petal length (cm) 4. Petal width (cm)

We use KNN to predict the species of a flower based on these features.

⸻

## Project Goals

    1.	Load and explore the Iris dataset using Pandas
    2.	Visualize data with Matplotlib (scatter plots, pair plots)
    3.	Split data into training and testing sets with stratified sampling
    4.	Implement KNN classification using sklearn
    5.	Visualize decision boundaries in 2D (petal length vs petal width)
    6.	Experiment with different values of k to see effects on accuracy and boundaries

⸻

## Technologies Used

    •	Python 3.12
    •	Pandas → for data handling
    •	Matplotlib → for plotting and visualizing data
    •	scikit-learn → for KNN, train/test split, accuracy evaluation

⸻

## Project Structure

IrisIndetification/
│
├─ .gitignore # Ignore unnecessary files
├─ README.md # Project overview (this file)
├─ iris_knn.ipynb # Main notebook with KNN implementation
└─ requirements.txt # Project dependencies

## How It Works

⸻

### Step 1: Load Data

    •	Load the Iris dataset from sklearn.datasets
    •	Convert it into a Pandas DataFrame for easy exploration

### Step 2: Visualize Data

    •	Scatter plots for individual features
    •	Pair plots for feature combinations
    •	Helps identify which features separate species best

### Step 3: Train/Test Split

    •	80% training, 20% testing
    •	stratify=y ensures all species are represented proportionally
    •	random_state=42 makes the split reproducible

### Step 4: Train KNN Classifier

    •	Choose k neighbors (default k=3)
    •	Fit the model on training data
    •	Predict species for test set

### Step 5: Evaluate Accuracy

    •	Compare predictions against actual labels
    •	Calculate accuracy using .score()

### Step 6: Visualize Decision Boundaries

    •	Use only 2 features (petal length and width) for 2D visualization
    •	Create a meshgrid of points covering feature space
    •	Predict species for each point to color the background
    •	Overlay training points on top

⸻

## Notes / Learning Points

    •	KNN is instance-based learning → it stores training points and predicts using neighbors
    •	Small k → more flexible, sensitive to noise
    •	Large k → smoother predictions, can underfit
    •	Stratified train/test split prevents class imbalance
    •	Decision boundaries show how KNN classifies feature space
