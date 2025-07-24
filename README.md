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

# Scatter plot
plt.figure(figsize=(8, 6))
sns.scatterplot(x='sepal_length', y='sepal_width', hue='species', data=iris)
plt.title('Sepal Length vs. Sepal Width')
plt.show()

# Histogram
plt.figure(figsize=(8, 6))
sns.histplot(iris['sepal_length'], bins=10, kde=True)
plt.title('Distribution of Sepal Length')
plt.show()

# Box plot
plt.figure(figsize=(8, 6))
sns.boxplot(x='species', y='petal_length', data=iris)
plt.title('Petal Length Across Species')
plt.show()
