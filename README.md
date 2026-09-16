 
 
 
  
Name: 
Register Number:  
Course Code: ITA04 
Course Name: Statistics with R Programming 
Faculty Name:  
 
1. Create numeric, character, and logical vectors and display type and content. 
 
Aim: 
To create numeric, character, and logical vectors and display type and content. 
 
Procedure: 
Step 1: Open RStudio or R console on your system. 
Step 2: Create a numeric vector containing numerical values. 
Step 3: Display the contents of the numeric vector on the screen. 
Step 4: Use the class function to check and print the data type of the numeric vector. 
Step 5: Create a character vector containing names or text values. 
Step 6: Display the contents of the character vector. 
Step 7: Use the class function to identify and print the data type of the character vector. 
Step 8: Create a logical vector containing TRUE and FALSE values. 
Step 9: Display the logical vector on the screen. 
Step 10: Use the class function to print the data type of the logical vector. 
Step 11: Observe and note that numeric, character, and logical vectors each have distinct data types. 
 
 
a <- c(10, 20, 30, 40, 50)
b <- c("Apple", "Banana", "Mango", "Orange")
c <- c(TRUE, FALSE, TRUE, FALSE)
a
b
c

typeof(a)
typeof(b)
typeof(c) 
 
 
Result: 
Hence the output is verified successfully. 
 
2. Create labeled matrices (5×4, 3×3, 2×2) filled by row/column. 
 
Aim: 
To create labeled matrices (5×4, 3×3, 2×2) filled by row/column. 
 
Procedure: 
Step 1: Open RStudio or R console on your system. 
Step 2: Create a matrix by arranging a sequence of numbers into rows and columns. 
Step 3: Display the created matrix to check its elements and layout. 
Step 4: Create another matrix with a different size (for example, 3×3) to understand matrix creation with various dimensions. 
Step 5: Display the second matrix to verify its arrangement. 
Step 6: Create a smaller matrix (for example, 2×2) to observe how matrix size can vary. 
Step 7: Display the third matrix to view its content. 
Step 8: Observe that each matrix organizes elements in a rectangular form with equallength rows and columns. 
 
 a = matrix(1:20, nrow=5, ncol=4)
rownames(a) = paste0("R", 1:5)
colnames(a) = paste0("C", 1:4)
a
 	 
 
Result: 
Hence the output is verified Succeessfully. 
 
3. Write an R program to create and display a 3D array with specified rows, columns, and tables. 
 
Aim: 
To write an R program to create and display a 3D array with specified rows, columns, and tables. 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Create a sequence of numbers to be stored in a variable. 
Step 3: Use that sequence to create a multi-dimensional array by specifying dimensions such as number of rows, columns, and tables. 
Step 4: Store the created array in a variable. 
Step 5: Display the array to view all the elements arranged across multiple rows, columns, and layers. 
Step 6: Observe how an array in R can store data in more than two dimensions, unlike a matrix. 
 
 
 a = array(1:24, dim=c(3,4,2))
a
 
 
Result: 
Hence the output is verified successfully. 
 
4. Create arrays from vectors with dimension names, print specific elements. 
 
Aim: 
To create arrays from vectors with dimension names, print specific elements. 
 
Procedure: 
Step 1: Open RStudio or R console on your system. 
Step 2: Create a sequence of numbers and store it in a variable. 
Step 3: Use the array function to arrange these numbers into multiple dimensions by specifying the number of rows, columns, and tables. 
Step 4: Store the created array in a variable. 
Step 5: Display the entire array to view how the elements are arranged in each layer. 
Step 6: Access a specific element from the array using its row, column, and table position. 
Step 7: Print the selected element to verify correct indexing within the array. 
 
 
 a = array(1:8, dim=c(2,2,2))
print(a[2,1,2])
  
 
Result: 
Hence the output is verified successfully. 
 
5. Create and manipulate factor variables (e.g., women’s dataset heights, random LETTERS sample). 
 
Aim: 
Create and manipulate factor variables (e.g., women’s dataset heights, random LETTERS sample). 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Create a character vector containing categorical values such as height levels. 
Step 3: Convert the character vector into a factor to represent it as categorical data. 
Step 4: Display the factor to observe that R assigns internal numeric codes to each category. 
Step 5: Set a random seed value to ensure that the random sampling results remain the same each time you run the program. 
Step 6: Randomly generate a sample of leflers from A to E using the sample function. 
Step 7: Convert the generated leflers into a factor to represent them as categorical variables. 
Step 8: Print the factor to view the sampled categories and their assigned levels. 
 
 height = factor(c("Short", "Tall", "Medium", "Tall", "Short"))
height
levels(height)

letters = factor(sample(LETTERS, 5))
letters 

Result: 
Hence the output is verified successfully. 
 
6. Create an R list containing vectors, matrices, and functions; display contents. 
 
Aim: 
To create an R list containing vectors, matrices, and functions; display contents. 
 
Procedure 
Step 1: Open RStudio or R console on your system. 
Step 2: Create a numeric vector and store it in a variable. 
Step 3: Create a matrix by arranging numbers into specified rows and columns. 
Step 4: Define a simple function that performs a mathematical operation (for example, squaring a number). 
Step 5: Combine the vector, matrix, and function into a single list using the list function. 
Step 6: Assign appropriate names to each component in the list for befler readability. 
Step 7: Display the list to view all its components — the vector, matrix, and function — stored together in one structured object. 
 
 a = list(numbers=1:5, matrix=matrix(1:4,2,2), fun=function() 5^2)
a
a$fun()
 
Result: 
 
Hence the output is verified successfully. 
 
7. Write R programs for basic tasks: Factors of a number, generate a vector of 10 random integers between -50 and 50, print numbers 1–100 with FizzBuzz logic. 
 
Aim: 
To write R programs for basic tasks: Factors of a number, generate a vector of 10 random integers between -50 and 50, print numbers 1–100 with FizzBuzz logic. 
 
Procedure 
Step 1: Open RStudio or R console on your system. 
Step 2: Assign an integer value to a variable to represent the number for which factors are to be found. 
Step 3: Initialize an empty integer vector to store the factors. 
Step 4: Use a for loop to iterate through all numbers from 1 to the given number. 
Step 5: Inside the loop, use the modulus operator to check if the number divides evenly (remainder equals 0). 
Step 6: If the condition is true, append that value to the factors vector. 
Step 7: After the loop completes, print all the factors of the given number. 
Step 8: Set a random seed to ensure the random number generation gives reproducible results. 
Step 9: Generate and print 10 random integers within a specified range (−50 to 50). 
Step 10: Use another for loop to iterate from 1 to 100 and apply the FizzBuzz logic: 
Print “FizzBuzz” for numbers divisible by both 3 and 5. 
Print “Fizz” for numbers divisible only by 3. 
Print “Buzz” for numbers divisible only by 5. 
Otherwise, print the number itself. 
Step 11: Display the complete sequence of printed outputs to verify the logic. 
 
 n = 12
factors = 1:n[n %% 1:n == 0]
print(factors)
x = sample(-50:50, 10)
print(x)
for(i in 1:100) {
  if(i %% 15 == 0) print("FizzBuzz")
  else if(i %% 3 == 0) print("Fizz")
  else if(i %% 5 == 0) print("Buzz")
  else print(i)
}
 
 
8) Generate random numbers from a normal distribution; count occurances
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Set a random seed value to make the random results reproducible every time you run the program. 
Step 3: Generate a set of random numbers from a normal distribution using the rnorm function. 
Step 4: Round the generated random numbers to the nearest whole number to group similar values. 
Step 5: Use the table function to count the frequency of each rounded value. 
Step 6: Convert the frequency table into a data frame for easier viewing and structured display. 
Step 7: Print the data frame to observe each rounded number along with its frequency count. 
 
 x = rnorm(100, mean=0, sd=1)
print(x)
table(round(x, 1))

Result: 
Hence the output is verified successfully. 
 
 
 
9. Create empty plots with specified axis limits. 
 
Aim: 
To create empty plots with specified axis limits. 
 
Procedure 
Step 1: Open RStudio or R console on your computer. 
Step 2: Remove the variable named c from the workspace using the remove function. 
Step 3: Use the plot function to create an empty graph by sefling the type as "n". 
Step 4: Define the range of x-axis and y-axis using xlim and ylim. 
Step 5: Label the x-axis and y-axis with appropriate names. 
Step 6: Run the program to display an empty plofling area ready for adding points or lines later. 
 
 plot(0, 0, type="n", xlim=c(0,10), ylim=c(0,10))
 
 
 
Result: 
Hence the output is verified successfully. 
 
10. Create and explore a data frame exam_data with name, score, attempts, and qualifying fields. Perform extract, add row/column, sort, save to file. 
 
Aim: 
To create and explore a data frame exam_data with name, score, aflempts, and qualifying fields. Perform extract, add row/column, sort, save to file. 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Create a data frame with student details such as name, score, aflempts, and qualification status. 
Step 3: Add a new student record to the existing data frame using the rbind function. 
Step 4: Add a new column named grade to assign grades for each student. 
Step 5: Arrange the data in descending order based on the score column. 
Step 6: Save the final data frame as a CSV file using the write.csv function. 
Step 7: Print the data frame to display the updated and sorted student information. 
 
 
 exam_data = data.frame(
  name = c("Arun", "Bala", "Cathy", "David"),
  score = c(85, 72, 90, 65),
  attempts = c(1, 2, 1, 3),
  qualifying = c(TRUE, TRUE, TRUE, FALSE)
)

exam_data

# Extract
exam_data$name
exam_data[1, ]

# Add a row
exam_data = rbind(exam_data, c("Esha", 78, 2, TRUE))

# Add a column
exam_data$grade = c("A", "B", "A", "C", "B")

# Sort by score
exam_data = exam_data[order(exam_data$score), ]

# Save to file
write.csv(exam_data, "exam_data.csv", row.names = FALSE)

exam_data

Result: 
Hence the output is verified successfully. 
 
11.	Write an R program to read a .csv file and display contents. 
 
Aim: 
To write an R program to read a .csv file and display contents. 
 
Procedure 
Step 1: Open RStudio or R console on your computer. 
Step 2: Use the read.csv function to load data from a CSV file into R. 
Step 3: Store the imported data in a variable for further use. 
Step 4: Display a message indicating that the file contents are being printed. 
Step 5: Print the data to view all the rows and columns from the CSV file. 
 
 data = read.csv("exam_data.csv")

print(data)

or
data = read.csv("C:/Users/YourName/Documents/exam_data.csv")
print(data)
 
Result: 
Hence the output is verified successfully. 
 
12.	Perform data reshaping on air quality dataset: melt, cast, compute monthly averages for Ozone, Solar.R, Wind, and Temperature. 
 
Aim: 
To perform data reshaping on air quality dataset: melt, cast, compute monthly averages for Ozone, Solar.R, Wind, and Temperature. 
 
Procedure 
Step 1: Open RStudio or R console on your computer. 
Step 2: Load the built-in dataset airquality available in R. 
Step 3: Use the aggregate function to calculate the mean of multiple columns (Ozone, Solar.R, Wind, and Temp) grouped by Month. 
Step 4: Include the parameter na.rm = TRUE to ignore any missing (NA) values while calculating averages. 
Step 5: Store the calculated monthly average values in a new variable. 
Step 6: Print a message to indicate that monthly averages are being displayed. 
Step 7: Display the result to view the average Ozone, Solar Radiation, Wind, and Temperature for each month. 
 
 library(reshape2)

data = airquality

# Melt
m = melt(data, id.vars = c("Month", "Day"))
print(m)

# Cast and calculate monthly averages
result = dcast(m, Month ~ variable, mean, na.rm = TRUE)
print(result)

install.packages("reshape2")

Result: 
Hence the output is verified successfully. 
 
13. Combine multiple arrays row-wise. 
 
Aim: 
To combine multiple arrays row-wise. 
 
Procedure 
Step 1: Open RStudio or R console on your system. 
Step 2: Remove all existing objects from the workspace using the rm function to start fresh. 
Step 3: Create three separate numeric vectors with values. 
Step 4: Combine all the vectors row-wise using the rbind function to form a matrix. 
Step 5: Print a message indicating that the arrays are combined row-wise. 
Step 6: Display the resulting matrix to view the combined data. 
 
 a = matrix(1:6, nrow=2, ncol=3)
b = matrix(7:12, nrow=2, ncol=3)

result = rbind(a, b)

print(result)
 
 
Result: 
Hence the output is verified successfully. 
 
14. Explore and manipulate ChickWeight dataset (sorting, melting, casting by Diet). 
 
Aim: 
To explore and manipulate ChickWeight dataset (sorting, melting, casting by Diet). 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Load the built-in dataset ChickWeight available in R. 
Step 3: Display the first few rows of the dataset using the head function to understand its structure. 
Step 4: Sort the dataset in ascending order based on the weight column using the order function. 
Step 5: Print the sorted dataset to view the records arranged by weight. 
Step 6: Use the aggregate function to calculate the average weight of chicks for each Diet group. 
Step 7: Display the result showing the mean weight corresponding to each diet type. 
 
 
 library(reshape2)

data = ChickWeight

# Display data
print(data)

# Sort by weight
data = data[order(data$weight), ]
print(data)

# Melt
m = melt(data, id.vars=c("Chick","Time","Diet"))
print(m)

# Cast by Diet
result = dcast(m, Diet ~ variable, mean, na.rm=TRUE)
print(result)
 
 
Result: 
Hence the output is verified successfully. 
 
15. Perform EDA on iris dataset: dimensions, summary, standard 
deviation,quantiles, grouping by Species, pivot table, categorical grouping with Sepal.Length categories. 
 
Aim: 
To perform EDA on iris dataset: dimensions, summary, standard deviation,quantiles, grouping by Species, pivot table, categorical grouping with Sepal.Length categories. 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Load the built-in dataset iris available in R. 
Step 3: Use the dim function to find the number of rows and columns in the dataset. 
Step 4: Apply the summary function to view basic statistical details such as minimum, maximum, mean, and quartiles for each variable. 
Step 5: Use the sapply function with sd to calculate the standard deviation of the numeric columns. 
Step 6: Find the quantile values of the Sepal.Length column to understand data distribution. 
Step 7: Use the aggregate function to calculate the mean of all numeric variables grouped by Species. 
Step 8: Display the results to observe the overall statistical analysis of the dataset. 
 
 data = iris

# Dimensions
dim(data)

# Summary
summary(data)

# Standard deviation
sapply(data[1:4], sd)

# Quantiles
sapply(data[1:4], quantile)

# Grouping by Species
aggregate(. ~ Species, data=data, mean)

# Pivot table
table(data$Species)

# Categorical grouping of Sepal.Length
data$Sepal.Category = cut(data$Sepal.Length,
                          breaks=c(4,5,6,7,8),
                          labels=c("Low","Medium","High","Very High"))

table(data$Sepal.Category)

Result: 
Hence the output is verified successfully. 
 
16. Explore USArrests dataset: summary statistics, state with largest rape arrests, max & min murder rates, correlation among features, states above median assault arrests and bottom 25% for murder, visualization with histogram, density, scatterplots, bar graphs. 
 
Aim: 
To explore USArrests dataset: summary statistics, state with largest rape arrests, max & min murder rates, correlation among features, states above median assault arrests and boflom 25% for murder, visualization with histogram, density, scaflerplots, bar graphs. 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Load the built-in dataset iris available in R. 
Step 3: Use the dim function to find the number of rows and columns in the dataset. 
Step 4: Apply the summary function to view basic statistical details such as minimum, maximum, mean, and quartiles for each variable. 
Step 5: Use the sapply function with sd to calculate the standard deviation of the numeric columns. 
Step 6: Find the quantile values of the Sepal.Length column to understand data distribution. 
Step 7: Use the aggregate function to calculate the mean of all numeric variables grouped by Species. 
Step 8: Display the results to observe the overall statistical analysis of the dataset. 
 
 data = USArrests

# Summary statistics
summary(data)

# State with largest rape arrests
rownames(data)[which.max(data$Rape)]

# Maximum and minimum murder rates
max(data$Murder)
min(data$Murder)

# Correlation among features
cor(data)

# States above median Assault arrests
data[data$Assault > median(data$Assault), ]

# Bottom 25% for Murder
data[data$Murder <= quantile(data$Murder, 0.25), ]

# Histogram
hist(data$Murder, main="Murder Arrests", xlab="Murder")

# Density plot
plot(density(data$Murder), main="Density of Murder")

# Scatterplot
plot(data$Murder, data$Assault,
     main="Murder vs Assault",
     xlab="Murder", ylab="Assault")

# Bar graph
barplot(data$Murder,
        names.arg=rownames(data),
        main="Murder Arrests",
        las=2)
 
 
Hence the output is verified successfully. 
 
17. Explore Titanic dataset: bar chart of survival vs class, modify plot by gender, histogram of Age. 
 
Aim: 
To explore Titanic dataset: bar chart of survival vs class, modify plot by gender, histogram of Age. 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Load the built-in dataset Titanic available in R. 
Step 3: Convert the Titanic dataset into a data frame format for easier manipulation and plofling. 
Step 4: Create a bar plot showing the relationship between Class and Survival using the table function to count frequencies. 
Step 5: Add a title to the plot to indicate that it represents Survival vs Class. 
Step 6: Create another bar plot to show the relationship between Gender and Survival. 
Step 7: Add an appropriate title for the second plot to represent Survival vs Gender. 
Step 8: Observe both plots to compare survival paflerns across different classes and genders. 
 
 data = read.csv("C:/Users/YourName/Downloads/titanic_train.csv")

barplot(table(data$Pclass, data$Survived),
        main="Survival vs Class",
        xlab="Class",
        ylab="Count",
        beside=TRUE)

barplot(table(data$Sex, data$Survived),
        main="Survival vs Gender",
        xlab="Gender",
        ylab="Count",
        beside=TRUE)

data$Age = as.numeric(as.character(data$Age))

hist(data$Age,
     main="Age Distribution",
     xlab="Age",
     na.rm=TRUE)
 
Result: 
Hence the output is verified successfully. 
 
18. Create graphs in R: boxplot, histogram, bar plot, line chart, scatter plot. 
 
Aim: 
To create graphs in R: boxplot, histogram, bar plot, line chart, scafler plot. 
 
Procedure: 
Step 1: Open RStudio or R console on your computer. 
Step 2: Create two numeric vectors containing values for plofling. 
Step 3: Use the par function with mfrow to divide the plofling area into multiple sections for displaying different charts together. 
Step 4: Draw a boxplot to show the distribution of the data. 
Step 5: Create a histogram to visualize the frequency of values. 
Step 6: Generate a bar plot with labeled bars to compare values across categories. 
Step 7: Plot a line chart to show the trend of values sequentially. 
Step 8: Draw a scafler plot to visualize the relationship between two numeric variables. 
Step 9: Observe all the graphs displayed in the multi-plot layout. 
 
 
 x = 1:10
y = c(2,5,4,8,6,9,7,10,8,12)

boxplot(y, main="Boxplot", ylab="Values")

hist(y, main="Histogram", xlab="Values")

barplot(y, main="Bar Plot", xlab="Values", ylab="Frequency")

plot(x, y, type="l", main="Line Chart", xlab="X", ylab="Y")

plot(x, y, main="Scatter Plot", xlab="X", ylab="Y")
 
Hence the output is verified successfully. 
 
19. Build a regression model on advertising dataset (Sales ~ Spend) and predict Sales. 
 
Aim: 
To build a regression model on advertising dataset (Sales ~ Spend) and predict Sales. 
 
Procedure 
Step 1: Open RStudio or R console on your computer. 
Step 2: Create two numeric vectors containing values for plofling. 
Step 3: Use the par function with mfrow to divide the plofling area into multiple sections for displaying different charts together. 
Step 4: Draw a boxplot to show the distribution of the data. 
Step 5: Create a histogram to visualize the frequency of values. 
Step 6: Generate a bar plot with labeled bars to compare values across categories. 
Step 7: Plot a line chart to show the trend of values sequentially. 
Step 8: Draw a scafler plot to visualize the relationship between two numeric variables. 
Step 9: Observe all the graphs displayed in the multi-plot layout. 
 
 Spend = c(10,20,30,40,50,60,70,80,90,100)
Sales = c(12,18,25,30,38,45,50,58,65,72)

data = data.frame(Spend, Sales)

print(data)

model = lm(Sales ~ Spend, data=data)

print(summary(model))

new_data = data.frame(Spend=50)

predicted_sales = predict(model, new_data)

print(predicted_sales)

plot(data$Spend, data$Sales,
     main="Sales vs Spend",
     xlab="Spend",
     ylab="Sales")

abline(model)
Result: 
Hence the output is verified successfully. 
 
20. Create multiple regression model using ChickWeight dataset with “Time” and “Diet” as predictors; predict weight and compute model error. 
 
Aim: 
To create multiple regression model using ChickWeight dataset with “Time” and “Diet” as predictors; predict weight and compute model error. 
 
Procedure 
Step 1: Open RStudio or R console on your computer. 
Step 2: Load the built-in dataset ChickWeight available in R. 
Step 3: Use the lm function to create a linear regression model where weight is predicted using Time and Diet as independent variables. 
Step 4: Use the predict function to generate predicted weight values based on the fifled model. 
Step 5: Calculate the mean squared error (MSE) by finding the average of squared differences between the actual and predicted weight values. 
Step 6: Display the calculated MSE to evaluate the accuracy of the regression model. 
 
 data = ChickWeight

model = lm(weight ~ Time + Diet, data=data)

print(summary(model))

predicted = predict(model, data)

print(predicted)

error = data$weight - predicted

print(error)

mse = mean(error^2)

print(mse)

rmse = sqrt(mse)

print(rmse)
 
 
Result: 
Hence the output is verified successfully. 
 
21. Randomly split iris dataset into train/test (80/20), build logistic regression (Species ~ Petal.Length + Petal.Width), predict, and evaluate with confusion matrix. 
 
Aim: 
To randomly split iris dataset into train/test (80/20), build logistic regression (Species ~ Petal.Length + Petal.Width), predict, and evaluate with confusion matrix. 
 
install.packages("nnet")
library(nnet)

set.seed(123)

data = iris

index = sample(1:nrow(data), 0.8*nrow(data))

train = data[index, ]
test = data[-index, ]

model = multinom(Species ~ Petal.Length + Petal.Width, data=train)

print(summary(model))

predicted = predict(model, test)

print(predicted)

confusion = table(Actual=test$Species, Predicted=predicted)

print(confusion)

accuracy = sum(diag(confusion)) / sum(confusion)

print(accuracy) 
