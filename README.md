# JavaScript Loose Typing Bug

This example demonstrates a common issue in JavaScript related to its loose typing system.  The `+` operator behaves differently depending on whether the operands are numbers or strings. If either operand is a string, it performs string concatenation rather than numerical addition.

## Bug
The `foo` function is intended to add two numbers. However, when one or both of the arguments are strings, it concatenates them instead.

## Solution
The solution involves explicitly converting the operands to numbers before performing the addition using `Number()` or `parseInt()`. This ensures consistent numerical behavior regardless of the input type.

## How to Reproduce
1. Copy `bug.js`.
2. Run it using a JavaScript interpreter (e.g., Node.js).
3. Observe the unexpected results.