# JavaScript Bug: Handling Null and Undefined in Arithmetic Operations

This repository demonstrates a common JavaScript bug related to the loose comparison operator (`==`) and how it can lead to unexpected results when performing arithmetic operations with `null` and `undefined` values.

## The Bug

The `foo` function is designed to add two numbers. However, it does not explicitly handle the cases where one or both of the input values might be `null` or `undefined`.  When `undefined` is used in an arithmetic operation, JavaScript produces `NaN`, which can propagate through your program and cause unexpected behavior.

## The Solution

The solution demonstrates the importance of using strict equality (`===`) and explicitly checking for `null` and `undefined` before performing the addition operation. This ensures the function behaves correctly in all scenarios, including when null or undefined values are encountered.

## How to run

1. Clone the repository.
2. Open `bug.js` to see the erroneous code.
3. Open `bugSolution.js` to see the corrected code.
4. Run both files using a JavaScript interpreter (such as Node.js) to observe the differences in output.