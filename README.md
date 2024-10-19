# 📚 Catalog Placements Assignment

**Duration:** 70 minutes  
**Language:** Any language except Python is allowed  
**Submission:** Push the code to GitHub and provide the link in the submission form.

---

## 📖 Problem Statement

In this assignment, you will work on a simplified version of **Shamir's Secret Sharing** algorithm.

### Polynomial Representation

Consider an unknown polynomial of degree \( m \). To solve for the coefficients, you need \( m + 1 \) roots, represented as \( k = m + 1 \).

An unknown polynomial of degree \( m \) can be represented as:

\[
f(x) = a_m x^m + a_{m-1} x^{m-1} + \ldots + a_1 x + c
\]

Where:
- \( f(x) \) is the polynomial function
- \( m \) is the degree of the polynomial
- \( a_m, a_{m-1}, \ldots, a_1, c \) are coefficients (real numbers)
- \( a_m \neq 0 \)

Your task is to find the constant term \( c \) of the polynomial using the given roots, provided in a specific JSON format.

---

## 📝 Input Format

The input is provided in JSON format, containing polynomial roots that need to be decoded based on their respective bases. 

### Sample Test Case

```json
{
    "keys": {
        "n": 4,
        "k": 3
    },
    "1": {
        "base": "10",
        "value": "4"
    },
    "2": {
        "base": "2",
        "value": "111"
    },
    "3": {
        "base": "10",
        "value": "12"
    },
    "6": {
        "base": "4",
        "value": "213"
    }
}
