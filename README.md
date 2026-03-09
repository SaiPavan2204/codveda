# Task 1: Basic Console Calculator

A simple, robust Java console application that performs fundamental arithmetic operations. This project was developed as part of a Java Development internship/learning path to demonstrate proficiency in basic Java syntax, method creation, and input handling.

---

## 🚀 Features

* **Four Core Operations:** Addition, Subtraction, Multiplication, and Division.
* **Edge Case Handling:** Includes logic to prevent crashes during division by zero.
* **User-Friendly Interface:** Clear console prompts and menu-driven selection.
* **Modular Design:** Each operation is handled by a dedicated static method for better readability and maintenance.

---

## 🛠️ Technical Implementation

The application is built using a single Java class `Calculator` that utilizes the following components:

### 1. Methods
To keep the code clean, every operation is mapped to a specific method:
* `add(double a, double b)`: Returns $a + b$
* `subtract(double a, double b)`: Returns $a - b$
* `multiply(double a, double b)`: Returns $a \times b$
* `divide(double a, double b)`: Returns $a / b$ with a check for $b = 0$.

### 2. Input Handling
We use the `java.util.Scanner` class to capture user input:
* `nextDouble()`: To allow for decimal calculations (e.g., $5.5 + 2.1$).
* `nextInt()`: To capture the user's menu choice.

### 3. Logic Flow
The program follows a linear execution path:
1.  **Input:** User enters two numbers.
2.  **Selection:** User chooses an operation (1-4).
3.  **Processing:** A `switch` statement calls the appropriate method.
4.  **Output:** The result is printed to the console.

---

## 💻 How to Run

1.  **Compile the code:**
    ```bash
    javac Calculator.java
    ```
2.  **Run the application:**
    ```bash
    java Calculator
    ```

---

## ⚠️ Error Handling
The program specifically addresses **Division by Zero**. If a user attempts to divide by zero:
1.  The `divide` method detects the divisor is `0`.
2.  An error message is displayed: `Error: Division by zero is not allowed.`
3.  The program prevents the calculation to avoid a `Runtime ArithmeticException`.
