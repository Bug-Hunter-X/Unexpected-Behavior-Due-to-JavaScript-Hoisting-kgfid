# Unexpected Behavior Due to JavaScript Hoisting

This repository demonstrates a common JavaScript error related to hoisting. The file `bug.js` shows code that leads to unexpected behavior, while `bugSolution.js` provides a corrected version. 

## Bug Description

The bug arises from using a variable before it has been initialized.  JavaScript's hoisting mechanism moves declarations to the top of their scope, but not initializations.  This results in the variable being accessed before it's assigned a value, causing `undefined` to be printed instead of the expected `10`.

## How to Reproduce

1. Clone the repository.
2. Open `bug.js` in a JavaScript environment (browser console, Node.js).
3. Run the `myFunc` function.  Observe the output in console.

## Solution

The solution involves ensuring the variable is initialized before it's used, as demonstrated in `bugSolution.js`.