# PHP Notice: A non well formed numeric value encountered
This repository demonstrates a common PHP error: "A non well formed numeric value encountered".  The error arises when attempting arithmetic operations on values that are not properly formatted as numbers. The `calculateSum` function showcases this issue, and the solution provides a robust way to handle potential non-numeric input.

## Bug
The `bug.php` file contains a function `calculateSum` that intends to add numbers from an array.  However, when the array contains a string that cannot be interpreted as a number, a PHP notice is thrown, and the result is incorrect.

## Solution
The `bugSolution.php` file provides an improved version of `calculateSum`.  It uses `is_numeric` to check if each element is a number before performing the addition. If an element is not numeric, it is skipped, ensuring that the function continues to work correctly even with mixed data types.