# Unexpected String Concatenation in JavaScript

This repository demonstrates a common JavaScript bug involving unexpected string concatenation due to type coercion.

## Bug Description
In JavaScript, when performing addition with a mix of string and number types, the `+` operator performs string concatenation instead of numerical addition. This behavior can lead to unexpected results if not handled carefully.

## How to Reproduce
1. Clone the repository.
2. Run `bug.js` using Node.js or a similar JavaScript runtime. 
3. Observe that the output is "12" instead of the expected 3.

## Solution
The solution involves explicit type conversion using `parseInt()` or `Number()` to ensure both operands are numbers before performing the addition, as shown in `bugSolution.js`.