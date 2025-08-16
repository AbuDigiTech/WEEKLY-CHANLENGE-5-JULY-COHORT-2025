# WEEKLY-CHANLENGE-5-JULY-COHORT-2025

# Import necessary libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import requests

# Task 1: Create a NumPy array and calculate the mean
numbers = np.arange(1, 11)
mean_value = np.mean(numbers)
print(f"Mean of numbers from 1 to 10: {mean_value}")

# Task 2: Load a dataset into a pandas DataFrame and display summary statistics
data = {
    'Name': ['Alice', 'Bob', 'Charlie', 'David', 'Emily'],
    'Age': [20, 21, 19, 22, 20],
    'Grade': [85, 90, 78, 92, 88]
}
df = pd.DataFrame(data)
print("\nSummary statistics:")
print(df.describe())

# Task 3: Fetch data from a public API and print a key piece of information
response = requests.get('https://jsonplaceholder.typicode.com/todos/1')
data = response.json()
print(f"\nTitle of the todo item: {data['title']}")

# Task 4: Plot a simple line graph
numbers = [1, 2, 3, 4, 5]
squares = [1, 4, 9, 16, 25]
plt.plot(numbers, squares)
plt.xlabel('Numbers')
plt.ylabel('Squares')
plt.title('Line Graph of Squares')
plt.show()
