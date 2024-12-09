# Off-by-One Error in Java Array

This repository demonstrates a common off-by-one error in Java when iterating through an array.  The `Bug.java` file contains the erroneous code, which attempts to access an array element beyond its bounds. The corrected code is provided in `BugSolution.java`.

## Problem Description

The code iterates through an integer array using a `for` loop. The loop condition `i <= arr.length` is incorrect; it should be `i < arr.length`. As a result, the code attempts to assign a value to `arr[5]` which is outside the valid index range of 0-4, resulting in an `ArrayIndexOutOfBoundsException`.

## Solution

The `BugSolution.java` file fixes this error by modifying the loop condition to `i < arr.length`. This ensures that the loop iterates only up to the last valid index of the array.