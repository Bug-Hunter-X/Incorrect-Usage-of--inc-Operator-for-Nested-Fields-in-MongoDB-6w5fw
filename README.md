# Incorrect Usage of $inc Operator for Nested Fields in MongoDB

This example demonstrates an uncommon error in MongoDB: incorrectly updating a nested field using the `$inc` operator. Using the dot notation correctly within the `$inc` operator is crucial for achieving the intended update in nested documents.

## Bug
The provided code snippet attempts to increment a nested field using `$inc`, but it fails to use dot notation correctly, leading to an incorrect update. This often results in an unintended or no update at all.

## Solution
The solution uses the dot notation correctly inside the `$inc` operator.  This notation correctly targets the nested field, ensuring proper incrementation.

## Usage
1. Clone this repository.
2. Ensure MongoDB is running.
3. Create a collection named `myCollection` and insert a document with a nested field.
4. Run the `bug.js` to see the incorrect behavior.
5. Then run `bugSolution.js` to see the correct way to update.