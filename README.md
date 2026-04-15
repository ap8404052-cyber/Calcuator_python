# 🧮 Python Calculator

This is a simple calculator program written in Python. It performs basic arithmetic operations like addition, subtraction, multiplication, and division.

---

## 🚀 Features
- Add two numbers
- Subtract two numbers
- Multiply two numbers
- Divide two numbers
- Continuous calculations using a loop

---

## 🧾 Code

```python
while True:
    try:
        num1 = float(input("\nEnter first number: "))
        num2 = float(input("Enter second number: "))

        op = input("Enter operation (+, -, *, /): ")

        if op == '+':
            print("Result:", num1 + num2)

        elif op == '-':
            print("Result:", num1 - num2)

        elif op == '*':
            print("Result:", num1 * num2)

        elif op == '/':
            if num2 != 0:
                print("Result:", num1 / num2)
            else:
                print("Error: Cannot divide by zero")

        else:
            print("Invalid operation")

    except ValueError:
        print("Error: Please enter valid numbers")

    again = input("Do you want to continue? (y/n): ")
    if again.lower() != 'y':
        print("Goodbye!")
        break
