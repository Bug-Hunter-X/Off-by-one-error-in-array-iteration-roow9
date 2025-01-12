# Off-by-One Error in Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over an array.  The error occurs when the loop index goes beyond the valid bounds of the array, resulting in an `ArrayIndexOutOfBoundsException`.  The solution demonstrates the correct way to iterate to avoid this error.

## Bug
The `Bug.java` file contains the code with the off-by-one error. The loop condition `i <= arr.length` is incorrect; it should be `i < arr.length`.  This causes an attempt to access `arr[5]` in an array of size 5, which is out of bounds.

## Solution
The `BugSolution.java` file provides the corrected code.  The loop condition is changed to `i < arr.length`, preventing the access of an invalid index.
