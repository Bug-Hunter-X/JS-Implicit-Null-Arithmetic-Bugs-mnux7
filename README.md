# Uncommon JavaScript Bug: Implicit Null Handling in Arithmetic Operations

This repository demonstrates a subtle bug in JavaScript related to how null values are handled in arithmetic operations.  The `bug.js` file shows the buggy code, while `bugSolution.js` provides a corrected version.

## Bug Description
The `foo` function is designed to add two numbers. However, it fails to explicitly handle cases where one or both of the input parameters are null.  In JavaScript, an attempt to perform arithmetic with null results in a type coercion to 0, but this might not be the desired behavior in all scenarios.

## Solution
The corrected code in `bugSolution.js` explicitly checks for null values and handles them appropriately, ensuring that the function returns the expected output or a meaningful indication of an error.

## Lessons Learned
This example highlights the importance of explicit null handling in JavaScript to avoid unexpected type coercion and ensure the reliability and predictability of your code.  Always consider the potential for null or undefined values in your function parameters and handle these cases explicitly.