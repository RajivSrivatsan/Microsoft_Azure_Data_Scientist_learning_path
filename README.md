# Microsoft_Azure_Data_Scientist_learning_path
All the learnings required to clear Microsoft Azure Data Science Associate certification

#Introduction

A data analysis project is designed to establish insights around a particular scenario or hypothesis

e.g. The relationship between amount of studying time of a student and final grade achieved.

# Learning Objectives

-Common data exploration and analysis tasks
-How to use Python packages like numPy, Pandas and Matplotlib to analyze data

# Explore data with NumPy and Pandas

These python packages are used for data procesing

# NumPy

NumPy is a python library that gives functionality that is equal to MATLAB and R. 

# Pandas

It is used for Data analysis and manipulation. Pandas is like Excel for Python

# Testing hypothesis

Data exploration and analysis is an iterative process, in which the data scientist takes a sample data and performs following tasks and tests the hypothesis:

- Clean data
- Apply statistical techniques to better understand the data
- Visualize data
- Revise the hypothesis and repeat the process

# Excercise - Explore Data with NumPy and Pandas

import numpy as np

this paackage is used for numerical operations, for instance if there is a list 

list =[1,2,3]

if,

list = list * 2

the output will be a list of [1,2,3,1,2,3]

The entire list will be repeated again.

But if the same data is stored in an numpy aray

data = np.array([1,2,3])

data = data * 2

the output will be an array of [2,4,6]

numpy array multiplies item wise whereas list multiplies the sequence.

=> type(data) will show it is an numpy array
=> data.shape - returns the number of rows and columns in the data, in this case, 1 x 3
=> data[0] - returns the first element of the array
=> data.mean() - returns the average of all elements in the array

To access the elements of 2D array,

data[0][0] can be used to get the first element

# Exploring Tabular Data with Pandas

A DataFrame can be used when there are multiple columns and rows
student_data = ([study_hours,grades])

df.student = pd.dataframe({'Name': ['Dan', 'Ross'],
'study_hours': student_data[0],
'Grade': student_data[1]})

# Finding and filtering data in a dataframe

you can use dataframe's loc method to retrieve data for a specific index value

df.student.loc[5]

you can also get data from a range of index values

df_student.loc[0:5]

You can also use iloc method to get data based on ordinal position of the value rather than the index

df_student.iloc[0:5]

iloc method can be used for retrieving values from rows to columns

for example, 

df_student.iloc[0,[1,2]]

the output will be the values in row 0, and column 1 and 2



