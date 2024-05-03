# PRODIGY_DS_01
# Task 1: Analyzing Product Name Distribution

## Description
This task involves analyzing the distribution of product names from an Excel file and visualizing the distribution using a bar chart.

## Requirements
- Python 3.x
- pandas
- matplotlib

## Installation
1. Install Python if you haven't already. You can download it from [here](https://www.python.org/downloads/).
2. Install pandas using pip:
3. 3. Install matplotlib using pip:


## Usage
1. Make sure you have the `data.xlsx` file in the same directory as your Python script.
2. Run the provided Python script `analyze_product_distribution.py`.
3. View the generated bar chart displaying the distribution of product names.

## Files
- `analyze_product_distribution.py`: Python script for analyzing product name distribution.

## Example
```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the data from the Excel file
data = pd.read_excel("data.xlsx")

distribution = data['PROD_NAME'].value_counts()

# Plotting the distribution as a bar chart
plt.figure(figsize=(15, 8))
distribution.plot(kind='bar')
plt.title('Distribution of Product Names')
plt.xlabel('Product Name')
plt.ylabel('Frequency')
plt.xticks(rotation=90)  # Rotate x-axis labels for better readability
plt.tight_layout()
plt.show()

