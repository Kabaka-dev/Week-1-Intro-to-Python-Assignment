# Week-1-Intro-to-Python-Assignment
Introduction to Python-Assignment 1(Python Calculator)
Intro to Python Assignment
Description - Instructions:

Basic Calculator Program

Create a simple Python program that asks the user to input two numbers and a mathematical operation (addition, subtraction, multiplication, or division).
Perform the operation based on the user's input and print the result.
Example: If a user inputs 10, 5, and +, your program should display 10 + 5 = 15.

How to Run the Program
1. Copy the code into a Python environment or a text editor and save it as calculator.py.
2. Run the script using Python: python calculator.py.
3. Follow the prompts to enter two numbers and a mathematical operation.

# Function to perform the mathematical operation
def calculate(num1, num2, operation):
    if operation == '+':
        return num1 + num2
    elif operation == '-':
        return num1 - num2
    elif operation == '*':
        return num1 * num2
    elif operation == '/':
        if num2 != 0:
            return num1 / num2
        else:
            return "Error: Division by zero is not allowed."
    else:
        return "Error: Invalid operation."

# Main program
def main():
    # Ask the user for input
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    operation = input("Enter the operation (+, -, *, /): ")

    # Perform the calculation
    result = calculate(num1, num2, operation)

    # Display the result
    print(f"{num1} {operation} {num2} = {result}")

# Run the program
if __name__ == "__main__":
    main()

