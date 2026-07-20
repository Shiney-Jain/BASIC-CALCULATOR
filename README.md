# BASIC-CALCULATOR
I have a created a basic calculator using python and also with the help of gemini as my first project . 
This are my codes for making it.
# Functions for basic mathematical operations
def add(x, y): return x + y
def subtract(x, y): return x - y
def multiply(x, y): return x * y
def divide(x, y): return x / y if y != 0 else "Error! Division by zero."

def calculator():
    print("--- Welcome to the Python Calculator ---")
    while True:
        print("\nOperations: 1(+), 2(-), 3(*), 4(/), 5(Quit)")
        choice = input("Enter choice (1-5): ").strip()
        if choice == '5': break
        if choice not in ('1', '2', '3', '4'):
            print("Invalid input!"); continue
        try:
            n1, n2 = float(input("Num 1: ")), float(input("Num 2: "))
            ops = {'1': add, '2': subtract, '3': multiply, '4': divide}
            print(f"Result: {ops[choice](n1, n2)}")
        except ValueError: print("Error! Please enter numbers.")

if __name__ == "__main__": calculator()


thank you !!
