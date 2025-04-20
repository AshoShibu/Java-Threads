
# Java Threads Project - Calculator Application

## Project Overview
This project demonstrates the working of Java threads in a simple calculator application. The program allows the user to perform basic mathematical operations (addition, subtraction, multiplication, division) using threads to execute the operations concurrently. 

### Main Features:
1. **Addition**
2. **Subtraction**
3. **Multiplication**
4. **Division**

Each of these operations is executed in a separate thread, allowing the program to handle them concurrently. The program provides a simple command-line interface where the user can choose an operation, input numbers, and see the results.

---

## Files in the Project

### 1. `OperationTask.java`
This class implements the `Runnable` interface to perform the four mathematical operations (addition, subtraction, multiplication, and division). 
Each operation is defined in the `run` method, and based on the user’s choice, the respective operation is executed in a separate thread.

#### Key Methods:
- **`run()`**: This method performs the requested operation and prints the result. It handles:
  - Addition (a + b)
  - Subtraction (a - b)
  - Multiplication (a * b)
  - Division (a / b, with division by zero check)

### 2. `Main.java`
This is the entry point of the program where the user interacts with the application. The user is presented with a menu to select an operation, and based on the selection, the corresponding operation is executed in a new thread.

#### Key Methods:
- **`main(String[] args)`**: The main method displays the menu, receives user input, and starts a new thread for the selected operation. It also ensures that the program continues running until the user selects the "Exit" option.

---

## How to Run:
1. Compile the Java files:
   ```
   javac OperationTask.java Main.java
   ```

2. Run the `Main` class:
   ```
   java Main
   ```

3. Follow the on-screen prompts to perform calculations.


