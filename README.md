# Incorrect Usage of MongoDB's $inc Operator
This repository demonstrates a common error when using the `$inc` operator in MongoDB.  The `$inc` operator is designed to increment a numeric field by a specified value.  However, providing a string value leads to an error.

## The Bug
The provided `bug.js` file contains code that attempts to increment the 'age' field of a document by the string value "10". This causes the MongoDB operation to fail.

## The Solution
The corrected code is located in `bugSolution.js`. This version correctly uses a numerical value to increment the 'age' field.  This ensures a successful update operation.

## How to reproduce
1. Clone this repository.
2. Ensure a MongoDB instance is running and you have the correct connection string.
3. Run `bug.js`. This will produce an error.
4. Run `bugSolution.js`. This will successfully update the document.  (You may need to modify the connection string according to your environment)