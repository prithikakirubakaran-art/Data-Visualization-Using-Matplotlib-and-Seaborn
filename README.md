# Experiment 2: Data Visualization Using Matplotlib and Seaborn

## Aim

To visualize data using Matplotlib and Seaborn libraries.

## Algorithm

1.  **Start.**
2.  Import the Matplotlib and Seaborn libraries.
3.  Load data into a Pandas DataFrame.
4.  Plot a histogram for age distribution using `plt.hist()`.
5.  Plot a scatter plot for Age vs. Salary using `sns.scatterplot()`.
6.  Plot salary distribution using `sns.boxplot()`.
7.  Show the plots sequentially.
8.  **Stop.**


## Program


    import pandas as pd
    import matplotlib.pyplot as plt
    import seaborn as sns

# Create dataset
    data = {
       'Age': [22, 25, 28, 30, 35, 40, 45, 50],
       'Salary': [20000, 25000, 30000, 35000, 40000, 45000, 50000, 60000]
      }

# Create DataFrame
    df = pd.DataFrame(data)

# Histogram for Age Distribution
    plt.figure(figsize=(6, 4))
    plt.hist(df['Age'], bins=5, color='skyblue', edgecolor='black')
    plt.title('Age Distribution')
    plt.xlabel('Age')
    plt.ylabel('Frequency')
    plt.show()

# Scatter Plot for Age vs Salary
    plt.figure(figsize=(6, 4))
    sns.scatterplot(x='Age', y='Salary', data=df)
    plt.title('Age vs Salary')
    plt.xlabel('Age')
    plt.ylabel('Salary')
    plt.show()

# Boxplot for Salary Distribution
    plt.figure(figsize=(6, 4))
    sns.boxplot(y='Salary', data=df)
    plt.title('Salary Distribution')
    plt.ylabel('Salary')
    plt.show()




## output
The program generates three separate graphical outputs in the following order.

1. Histogram – Age Distribution
 <img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/f2ba6341-574a-49fa-9848-4ff7b289b22e" />

X-axis: Age
Y-axis: Frequency
Displays the distribution of employees' ages.

2. Scatter Plot – Age vs Salary
 <img width="597" height="357" alt="image" src="https://github.com/user-attachments/assets/cade0d9e-6369-4b5f-8412-fc980f6f47a3" />

- X-axis: Age
- Y-axis: Salary
- Shows the relationship between age and salary.
  
3. Boxplot – Salary Distribution
  <img width="558" height="355" alt="image" src="https://github.com/user-attachments/assets/ceff06ad-0511-4936-9c66-fba2a80b12ce" />

## result
Thus, the data visualization program was successfully executed using Matplotlib and Seaborn libraries. The histogram, scatter plot, and boxplot were generated to visualize age distribution, the relationship between age and salary, and salary distribution respectively.

