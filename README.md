# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB.  The `$inc` operator is used to increment a numerical field by a specified value.  However, if a string is provided instead of a number, MongoDB will not perform the incrementation correctly, potentially leading to unexpected results or errors.

## Bug
The bug lies in the incorrect usage of the `$inc` operator.  A string value ("1") is used instead of a number (1), causing the update operation to fail or produce unexpected results. 

## Solution
The solution involves ensuring that the value provided to `$inc` is a valid number.  This can be accomplished by using a numerical literal or a variable that holds a numerical value.