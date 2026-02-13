# **Experiment 6: Study of conditional statements in Python**

## **Aim :**
To study and implement conditional statements in Python and understand decision-making using various conditional constructs.

## **Objectives :**
To understand the concept of conditional statements

To implement if, if-else, and if-elif-else statements

To use nested conditional statements

To apply conditional statements in real-life programming scenarios

## **Theory on Conditional Statements :**
Conditional statements in Python are used to control the flow of a program by making decisions based on whether certain conditions are true or false. They use keywords such as if, elif, and else to execute different blocks of code depending on the outcome of a condition, which is evaluated as a Boolean value (True or False). 

The if statement checks a condition and runs the corresponding code if it is true, while else provides an alternative block if the condition is false, and elif allows multiple conditions to be tested sequentially. 

These statements often use comparison operators like ==, !=, >, <, >=, <= and logical operators such as and, or, and not to form complex conditions. Indentation is essential in Python because it defines the scope and structure of conditional blocks, ensuring the program executes correctly.

## **Types of Conditional Statements :**

if statement

if-else statement

if-elif-else statement

Nested if statement

### **Program 1: Simple if Statement**
num = 10

if num > 0:

print("The number is positive")

### **Program 2: if-else Statement**

num = -5

if num >= 0:

print("The number is positive or zero")

else:

print("The number is negative")

### **Program 3: if-elif-else Statement**

marks = 75

if marks >= 90:

print("Grade: A")

elif marks >= 75:

print("Grade: B")

elif marks >= 50:

print("Grade: C")

else:

print("Grade: Fail")

### **Program 4: Nested if Statement**

num = 15

if num > 0:

if num % 2 == 0:

print("Positive Even number")

else:

print("Positive Odd number")

else:

print("Negative number")

## **Applications of Conditional Statements**
Decision-making in programs

Validating user input

Menu-driven programs

Checking eligibility (age, marks, etc.)

Control flow in real-world applications

## **Conclusion :**
Conditional statements form the backbone of decision-making in Python programs. By using if, if-else, elif, and nested conditions, programs can respond intelligently to different situations, making Python powerful and flexible for real-life applications.
