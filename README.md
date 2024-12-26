# JavaScript Unexpected String Concatenation Bug
This repository demonstrates a common, yet subtle, bug in JavaScript related to unexpected string concatenation.  The `foo` function intends to add two numbers, but due to type coercion, it performs string concatenation instead when one of the inputs is a string.

## Bug Report
The `bug.js` file contains the buggy code.  The function `foo` should add two numbers, but it produces an unexpected result when one argument is a string.

## Solution
The `bugSolution.js` file demonstrates a solution using type checking to ensure both inputs are numbers before performing addition.  Alternatively, `parseInt` or `Number` could be used for explicit type conversion if appropriate.

## How to Reproduce
1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js` to observe the unexpected output.
4. Run `node bugSolution.js` to see the corrected output.