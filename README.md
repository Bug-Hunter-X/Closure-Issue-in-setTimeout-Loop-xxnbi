# Closure Issue in setTimeout Loop

This repository demonstrates a common JavaScript error related to closures within loops using `setTimeout`.

The `bug.js` file contains the buggy code.  The loop intends to print numbers 0-9 with a one-second delay between each. However, due to the way closures work in JavaScript, it will instead print '10' ten times.

The `bugSolution.js` file provides a solution using an immediately invoked function expression (IIFE) to create a new scope for each iteration, capturing the correct value of `i`.

This example highlights the importance of understanding how closures function in JavaScript, particularly when dealing with asynchronous operations.