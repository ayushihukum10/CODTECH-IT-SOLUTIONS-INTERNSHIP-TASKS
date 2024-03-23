**Title: CODTECH-IT-SOLUTIONS-INTERNSHIP-TASK Documentation : SIMPLE CALCULATOR WITH ADVANCE FEATURES**
**Introduction:** 
The task is SIMPLE CALCULATOR WITH ADVANCE FEATURES

This Python program implements a user-friendly calculator that offers basic arithmetic operations (addition, subtraction, multiplication, division) along with exponentiation and the ability to quit. It adheres to good programming practices for clarity, maintainability, and error handling.

**Intern Information :**
NAME : AYUSHI HUKUM 
INTERN ID : COD4449

**Task Description:**
The task assigned to Ayushi Hukum during codtech it solutions internship program is to Write a python program for simple calculator with advance features,which implements a simple calculator with advanced features such asaddition, subtraction, multiplication, division, exponentiation, andthe option to quit. Study the code and explain how the programworks, including its main features and functionality
**Implementation:**

The code defines several functions for specific tasks and utilizes the main function to manage the user interaction and program flow. It ensures robust input handling and error management for division by zero.


def add(x, y):
  """Adds two numbers."""
  return x + y

def subtract(x, y):
  """Subtracts two numbers."""
  return x - y

def multiply(x, y):
  """Multiplies two numbers."""
  return x * y

def divide(x, y):
  """Divides two numbers, handling division by zero."""
  if y == 0:
    print("Error: Division by zero is not allowed.")
    return None
  return x / y

def exponentiate(x, y):
  """Raises a number to a power."""
  return x ** y

def get_user_input(prompt):
  """Gets user input as a float."""
  while True:
    try:
      return float(input(prompt))
    except ValueError:
      print("Invalid input. Please enter a number.")

def print_menu():
  """Prints the calculator menu."""
  print("\nSimple Calculator")
  print("1. Add")
  print("2. Subtract")
  print("3. Multiply")
  print("4. Divide")
  print("5. Exponentiate")
  print("6. Quit")

def add(x, y):
  """Adds two numbers."""
  return x + y

def subtract(x, y):
  """Subtracts two numbers."""
  return x - y

def multiply(x, y):
  """Multiplies two numbers."""
  return x * y

def divide(x, y):
  """Divides two numbers, handling division by zero."""
  if y == 0:
    print("Error: Division by zero is not allowed.")
    return None
  return x / y

def exponentiate(x, y):
  """Raises a number to a power."""
  return x ** y

def get_user_input(prompt):
  """Gets user input as a float."""
  while True:
    try:
      return float(input(prompt))
    except ValueError:
      print("Invalid input. Please enter a number.")

def print_menu():
  """Prints the calculator menu."""
  print("\nSimple Calculator")
  print("1. Add")
  print("2. Subtract")
  print("3. Multiply")
  print("4. Divide")
  print("5. Exponentiate")
  print("6. Quit")

def main():
  """The main function that runs the calculator."""
  while True:
    print_menu()
    choice = input("Enter your choice (1-6): ")

    if choice in ('1', '2', '3', '4', '5'):
      num1 = get_user_input("Enter the first number: ")
      num2 = get_user_input("Enter the second number: ")

      if choice == '1':
        result = add(num1, num2)
        print(f"{num1} + {num2} = {result}")
      elif choice == '2':
        result = subtract(num1, num2)
        print(f"{num1} - {num2} = {result}")
      elif choice == '3':
        result = multiply(num1, num2)
        print(f"{num1} * {num2} = {result}")
      elif choice == '4':
        result = divide(num1, num2)
        if result is not None:
          print(f"{num1} / {num2} = {result}")
      elif choice == '5':
        result = exponentiate(num1, num2)
        print(f"{num1} ^ {num2} = {result}")

    elif choice == '6':
      print("Exiting calculator...")
      break
    else:
      print("Invalid input. Please enter a number between 1 and 6.")

if _name_ == "_main_":
  main()


**code explanation :**
Functions:

add(x, y): This function adds two numbers x and y and returns the sum.
subtract(x, y): This function subtracts y from x and returns the difference.
multiply(x, y): This function multiplies x and y and returns the product.
divide(x, y): This function divides x by y. It checks for division by zero and prints an error message if encountered, returning None in that case. Otherwise, it returns the result of the division.
exponentiate(x, y): This function raises x to the power of y and returns the result.
get_user_input(prompt): This function prompts the user with a message (prompt) and keeps asking for input until a valid number (float) is entered.
print_menu(): This function prints the menu of the calculator with options for addition, subtraction, multiplication, division, exponentiation, and quitting.
main(): This is the main function of the program. It runs in a loop, continuously displaying the menu and asking the user for a choice.
Based on the user's choice, it calls the appropriate function (add, subtract, etc.) with user-provided numbers.
It handles division by zero error gracefully by checking the returned value from the divide function.
Choice '6' exits the loop and terminates the program.



**Rationale :**
calculate function: Encapsulates the calculation logic, promoting reusability and clarity. It handles basic arithmetic and exponentiation, raising ValueError for invalid operators or division by zero.
while loop: Creates a continuous loop for repeated calculations until the user chooses to quit.
User input: Prompts the user for a choice and validates it. If invalid, an error message is displayed, and the loop continues.
Number input: Handles potential non-numeric input with a try-except block, providing an error message and restarting the loop if necessary.
operator dictionary: Maps user choices (1-5) to their corresponding mathematical operators for easier lookup and clarity.
Calculation and result display: Uses the calculate function with the extracted operator to perform the calculation. The result is displayed, along with error handling for division by zero.
Quit option: The while loop terminates when the user chooses option 6 (Quit).



**Conclusion:**
The task is assigned to Ayushi Hukum during the codtech IT solutions internship program Involved "SIMPLE CALCULATOR WITH ADVANCE FEATURES" 
This Python program successfully implements a simple calculator with advanced features, providing a user-friendly experience for performing basic arithmetic operations (addition, subtraction, multiplication, division) and exponentiation. It incorporates the following key aspects:

Functionality: Offers a range of calculations that cater to common mathematical needs.
Error Handling: Gracefully handles invalid input (choices or numbers) and division by zero, providing informative error messages to the user.
User Friendliness: Presents a clear menu for selecting operations and guides the user through the calculation process.
Code Structure: Employs functions, loops, error handling, and data types effectively to create a well-organized and maintainable program.
This comprehensive approach ensures a robust and user-friendly calculator that can be easily extended to include additional features in the future.
this concludes the documentation for the task "SIMPLE CALCULATOR WITH ADVANCE FEATURES" assigned during the codtech IT solutions internship program
