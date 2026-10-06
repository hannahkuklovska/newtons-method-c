# Newton's Method for N-th Roots in C

A C implementation of Newton's method for approximating the n-th root of a number.

This project demonstrates iterative numerical computation, floating-point precision, custom mathematical functions, and pointer-based result handling in C.

## Overview

Newton's method is an iterative numerical technique used to approximate solutions to equations.

In this project, the method is used to calculate the n-th root of a number by repeatedly improving an initial estimate until the result reaches a specified error tolerance.

Instead of relying directly on a built-in root function, the approximation is calculated iteratively.

## Features

- Computes the n-th root of a number
- Implements Newton's method from scratch
- Includes a custom power function
- Supports positive and negative exponents
- Uses floating-point tolerance to determine convergence
- Demonstrates pointer-based output parameters
- Written in C
- Makefile-based compilation

## How It Works

To find the n-th root of a value `x`, the program solves:

```text
y^n = x
```

using Newton's iterative method.

The approximation is updated using:

```text
y(k+1) = ((n - 1) * y(k) + x / y(k)^(n - 1)) / n
```

Each iteration produces a more accurate estimate.

The process continues until the result reaches the required precision.

## Example

For:

```text
x = 16
n = 2
```

the result is approximately:

```text
4.0
```

For:

```text
x = 27
n = 3
```

the result is approximately:

```text
3.0
```

## Project Structure

```text
.
├── zadanie01.c
├── makefile
├── README.md
└── .gitignore
```

- `zadanie01.c` — implementation of Newton's method and supporting functions
- `makefile` — build configuration
- `README.md` — project documentation
- `.gitignore` — ignored files

## Building the Project

Clone the repository:

```bash
git clone https://github.com/hannahkuklovska/newtons-method-c.git
cd newtons-method-c
```

Compile the project:

```bash
make
```

Then run the generated executable.

## Concepts Demonstrated

This project demonstrates:

- C programming
- Iterative algorithms
- Numerical approximation
- Newton's method
- Floating-point arithmetic
- Convergence and error tolerance
- Functions
- Pointers
- Custom mathematical operations
- Makefiles

## What I Learned

Through this project, I practiced implementing a mathematical algorithm directly in C.

I also gained experience with:

- translating mathematical formulas into code,
- implementing iterative algorithms,
- working with floating-point precision,
- defining convergence conditions,
- passing results using pointers,
- and organizing a small C project with a Makefile.

## Possible Improvements

Future improvements could include:

- Better input validation
- Improved handling of edge cases
- Automated tests
- Command-line input
- Comparison with standard library results
- Support for additional numerical methods

## Author

Hannah Kuklovska
