# alumathunique

Matrix multiplication with personality and humor!  
A fun and educational Python package for matrix multiplication, featuring custom error messages from each group member.

---

## Installation

Install directly from PyPI:

bash
pip install alumathunique


Or, if you have the source code:

bash
pip install .


---

## Usage

python
from alumathunique.matrix_multiply import create_matrix, multiply_matrices

# Create matrices
A = create_matrix([[1, 2], [3, 4]])
B = create_matrix([[5, 6], [7, 8]])

# Multiply matrices
C = multiply_matrices(A, B)

# Print the result
print(C)


If you try to multiply matrices with incompatible dimensions, you’ll get a custom, humorous error message:

python
from alumathunique.matrix_multiply import create_matrix, multiply_matrices, MatrixMultiplicationError

A = create_matrix([[1, 2, 3], [4, 5, 6]])
B = create_matrix([[7, 8], [9, 10]])

try:
    C = multiply_matrices(A, B)
except MatrixMultiplicationError as e:
    print(e)


---

## Features

- Matrix class for 2D array operations
- Matrix multiplication with detailed, humorous error messages
- Easy-to-use API
- Custom exceptions for invalid operations

---

## Running Tests

To run the unit tests:

bash
pytest


---

## Project Structure

- alumathunique/ - Main package code
- tests/ - Unit tests
- setup.py - Packaging script
- README.md - This file

---

## Deployment link
https://pypi.org/project/alumathunique/0.1.0/

## Authors

Belyse, Elyse, Bella