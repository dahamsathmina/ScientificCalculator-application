# Scientific Calculator

<p align="center">
  <strong>A lightweight, interactive scientific calculator built with C# and .NET 8.</strong>
  <br />
  Perform everyday arithmetic and advanced mathematical calculations directly from your terminal.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/C%23-.NET%208-512BD4?logo=dotnet&logoColor=white" alt="C# and .NET 8" />
  <img src="https://img.shields.io/badge/APP-Console-1F6FEB" alt="Console application" />
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="MIT License" />
</p>

---

## Overview

**Scientific Calculator** is a menu-driven console application developed in C#. It brings basic arithmetic, scientific functions, and calculation-history tools together in a simple terminal interface.

The calculator supports operations such as addition, subtraction, multiplication, division, powers, square roots, factorials, trigonometry, logarithms, and exponential calculations. It also lets you review previous calculations and reuse the last result.

## Features

- **Basic arithmetic** — addition, subtraction, multiplication, division, and modulus.
- **Advanced mathematics** — powers, square roots, factorials, and absolute values.
- **Trigonometry** — sine, cosine, and tangent, with angles entered in degrees.
- **Logarithmic functions** — base-10 logarithm (`log`) and natural logarithm (`ln`).
- **Exponential function** — calculate `eˣ`.
- **Calculation history** — view or clear calculations from the current session.
- **Last-result reuse** — press Enter at a number prompt to use the previous result.
- **Console feedback** — color-coded results, errors, and notifications.
- **Input and domain checks** — includes checks for invalid menu choices, division by zero, negative square roots, and invalid logarithm inputs.

## Supported Operations

| Menu option | Operation | Description |
|---:|---|---|
| 1 | Addition (`+`) | Adds the entered numbers. |
| 2 | Subtraction (`-`) | Subtracts subsequent numbers from the first number. |
| 3 | Multiplication (`*`) | Multiplies the entered numbers. |
| 4 | Division (`/`) | Divides the first number by subsequent numbers. |
| 5 | Modulus (`%`) | Calculates the remainder. |
| 6 | Power (`^`) | Raises a base to a power. |
| 7 | Square root (`√`) | Calculates the square root of a non-negative number. |
| 8 | Factorial (`!`) | Calculates the factorial of a non-negative integer. |
| 9 | Sine (`sin`) | Calculates sine using degrees. |
| 10 | Cosine (`cos`) | Calculates cosine using degrees. |
| 11 | Tangent (`tan`) | Calculates tangent using degrees. |
| 12 | Logarithm (`log`) | Calculates the base-10 logarithm of a positive number. |
| 13 | Natural logarithm (`ln`) | Calculates the natural logarithm of a positive number. |
| 14 | Exponential (`eˣ`) | Calculates the exponential function. |
| 15 | Absolute value (`abs`) | Returns the non-negative magnitude of a number. |
| 16 | View history | Displays calculations from the current session. |
| 17 | Clear history | Clears the current session's calculation history. |
| 18 | Exit | Closes the calculator. |

## Requirements

- .NET 8.0 SDK or later
- Git (to clone the repository)
- A terminal or command prompt

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/dahamsathmina/ScientificCalculator-application.git
```

### 2. Open the project folder

```bash
cd ScientificCalculator-application
```

### 3. Restore and build

```bash
dotnet restore
dotnet build
```

### 4. Run the calculator

```bash
dotnet run
```

The calculator menu will appear in your terminal. Enter the number for the operation you want to perform.

## How to Use

1. Choose an operation from the menu by entering its option number.
2. For operations that accept multiple numbers, enter each number when prompted.
3. Type `done` and press Enter when you have finished entering numbers.
4. Press Enter at a number prompt to reuse the previous calculation result.
5. Select **16** to view the current session's history or **17** to clear it.
6. Select **18** to exit.

> **Note:** Trigonometric inputs are interpreted as degrees, not radians. Calculation history is kept in memory and is cleared when the application closes.

## Example Calculations

### Addition

```text
Select an operation: 1
Number: 5
Number: 10
Number: 15
Number: done
Result: 5 + 10 + 15 = 30
```

### Factorial

```text
Select an operation: 8
Number: 5
Number: done
5! = 120
```

### Square root

```text
Select an operation: 7
Enter a number: 16
√16 = 4
```

### Trigonometry

```text
Select an operation: 9
Number: 30
Number: done
sin(30°) = 0.5
```

## Project Structure

```text
ScientificCalculator-application/
│
├── Assets/                      # Project assets
├── Program.cs                   # Calculator logic and console interface
├── ScientificCalculator.csproj  # .NET project configuration
├── LICENSE                      # MIT License
└── README.md                    # Project documentation
```

## Technical Notes

- The application uses C# and the .NET `System` libraries.
- Calculations use the `double` numeric type for most mathematical operations.
- Factorial results are stored in a 64-bit integer; values greater than `20!` exceed that type's range.
- The application is interactive and runs in a terminal. It does not currently provide a graphical user interface.

## License

This project is licensed under the [MIT License](LICENSE).

---

<p align="center">
  Built with C# and .NET 8.
</p>
