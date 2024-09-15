# ECE2112-PA3 PYTHON DATA ANALYSIS (PANDAS)
Name: Supnet Joshua
Section: 2ECE-D
Date Submitted: September 17, 2024

# PROBLEM 1: Using knowledge obtained from the experiment and demonstrations:
A. Load the corresponding .csv file into a data frame named cars using pandas

B. Display the first five and last five rows of the resulting cars.
- To solve this problem, we must download and import a file called "cars.csv" first. Then we import pandas as pd to start solving this problem.
According to the problem, I must use the name cars as my data frame, so cars = cars.read_csv('cars.csv). The code "read_csv" is a code that allows loading of a CSV file into Python. This is in the form of Excel.
- I input the code "cars.head(5)". This will display the first five rows of cars. Then I also inputted the code "cars.tails(5)". This will display the last five rows of cars.
- Then I save the file name to Supnet_Pandas-P1 in .py
  
# PROBLEM 2: Using the dataframe cars in problem 1, extract the following information using subsetting, slicing and indexing operations.
a. Display the first five rows with odd-numbered columns (columns 1, 3, 5, 7...) of cars.
- For problem part a, I use splicing to get the first five rows with odd-numbered columns. The code for it is "cars[1:11:2]". "1" is the beginning of the splice. "11" is the end, excluding row 11. "2" is how many steps it will splice. This will display the first five rows that are odd numbers.
  
b. Display the row that contains the ‘Model’ of ‘Mazda RX4’.
- For problem part b, I use indexing to display the row. The code will be cars.loc[cars['Model']=='Mazda RX4']. So this will be located in the model of the data frame 'cars', which contains the name 'Mazda RX4'. This will display the row
  
c. How many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have?
- For problem part c, I also use indexing for this problem to find the number of 'cyl' of the car model 'Camaro Z28' has. The code will be cars.loc[cars['Model'] == 'Camaro Z28', ['Model','cyl']]. This is similar to the code in part b, but I use the model and cyl as a condition for it to be display as the output
  
d. Determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.
- For problem part d, similarly to part b and c, I use indexing but for 3 different models. The code will be A = cars.loc[cars['Model'] == 'Mazda RX4 Wag', ['Model','cyl','gear']]. For B, B = cars.loc[cars['Model'] == 'Ford Pantera L', ['Model','cyl','gear']]. For C, C = cars.loc[cars['Model'] == 'Honda Civic', ['Model','cyl','gear']]. Then we add print(A),print(B),print(C) for the displayed output.

# References
- You may use the images to know how I solved these problems and the uploaded codes.

# Updates
- Update 1: In Problem 1, the output gives an accurate but messy result. I separated the .head and .tail on a different cell to fix this.
- Update 2: In Problem 2, on part d comment, it is indexing, not slicing
- Update 3: In problem 2, The output for part d is messy, and it is best to separate each cell output to display tidy outputs. With this, the print code is removed and replaced with just variable outputs
