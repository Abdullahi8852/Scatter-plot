# Scatter-plot
To analyze relationships between variables
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the Iris dataset
iris = sns.load_dataset('iris')

# Display dataset structure
print("Dataset Shape:", iris.shape)
print("Dataset Columns:", iris.columns)
print("First Few Rows of the Dataset:")
print(iris.head())
