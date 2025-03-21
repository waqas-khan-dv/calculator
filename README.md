# Calculator

Welcome to the advanced calculator made in Python! This calculator has the ability to solve complex problems with ease. Below are the features and instructions on how to use it.

## Features

- Addition
- Subtraction
- Multiplication
- Division
- Exponentiation
- Modulus
- Square Root

## How to Use

1. **Addition**: Adds two numbers.
2. **Subtraction**: Subtracts the second number from the first number.
3. **Multiplication**: Multiplies two numbers.
4. **Division**: Divides the first number by the second number. (Note: Division by zero is not allowed.)
5. **Exponentiation**: Raises the first number to the power of the second number.
6. **Modulus**: Finds the remainder when the first number is divided by the second number.
7. **Square Root**: Finds the square root of a number. (Note: Square root of a negative number is not allowed.)

## Running the Calculator

To run the calculator, simply execute the Python script. Follow the on-screen instructions to perform various mathematical operations.

```python
import math

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Oops! Division by zero is not allowed."
    return x / y

def exponentiate(x, y):
    return x ** y

def modulus(x, y):
    return x % y

def square_root(x):
    if x < 0:
        return "Oops! Square root of a negative number is not allowed."
    return math.sqrt(x)

def calculator():
    print("Welcome to the Fun Calculator!")
    print("Let's do some math!")

    while True:
        print("\nChoose an operation:")
        print("1. Add")
        print("2. Subtract")
        print("3. Multiply")
        print("4. Divide")
        print("5. Exponentiate")
        print("6. Modulus")
        print("7. Square Root")
        print("8. Exit")

        choice = input("Enter choice (1/2/3/4/5/6/7/8): ")

        if choice == '8':
            print("Goodbye! Have a great day!")
            break

        if choice in ['1', '2', '3', '4', '5', '6']:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))

            if choice == '1':
                print(f"The sum of {num1} and {num2} is {add(num1, num2)}")
            elif choice == '2':
                print(f"The difference between {num1} and {num2} is {subtract(num1, num2)}")
            elif choice == '3':
                print(f"The product of {num1} and {num2} is {multiply(num1, num2)}")
            elif choice == '4':
                print(f"The result of dividing {num1} by {num2} is {divide(num1, num2)}")
            elif choice == '5':
                print(f"The result of {num1} raised to the power of {num2} is {exponentiate(num1, num2)}")
            elif choice == '6':
                print(f"The modulus of {num1} and {num2} is {modulus(num1, num2)}")
        elif choice == '7':
            num = float(input("Enter the number: "))
            print(f"The square root of {num} is {square_root(num)}")
        else:
            print("Invalid input! Please enter a number between 1 and 8.")

if __name__ == "__main__":
    calculator()
```

Enjoy using the advanced calculator!
