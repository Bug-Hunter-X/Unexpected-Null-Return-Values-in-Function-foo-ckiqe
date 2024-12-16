# Unexpected Null Return Values in Function foo

This repository demonstrates a common JavaScript bug involving unexpected null return values from a function that doesn't handle null input values robustly. The `foo` function is designed to add two numbers but returns null if either input is null.  While this might be intentional in some cases, it often leads to unexpected behavior and errors in larger applications.

## Bug Description

The `bug.js` file contains the function `foo`, which adds two numbers. However, if either input is null, the function immediately returns null, potentially causing issues downstream.

## Solution

The `bugSolution.js` file provides a corrected version of the function, handling null inputs gracefully by using a default value (0).  Alternatively, you could choose to throw an error to indicate that invalid input was provided.