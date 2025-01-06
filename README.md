# MongoDB $inc Operator with String Value

This example demonstrates an uncommon error in MongoDB when using the `$inc` operator with a string value instead of a number.  The `$inc` operator is designed to increment a numeric field by a specified value. Providing it with a string will cause the operation to fail silently or produce unexpected results.

## Bug
The provided `bug.js` demonstrates the incorrect usage of `$inc`. Attempting to increment a numerical field (`count`) with a string value ('1') leads to an unexpected outcome; the value of `count` will not increment correctly.

## Solution
The `bugSolution.js` file shows the corrected implementation.  The string '1' is replaced with a numerical value (1), ensuring the `$inc` operator functions as intended.