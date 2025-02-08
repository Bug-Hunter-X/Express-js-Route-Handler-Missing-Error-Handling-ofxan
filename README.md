# Express.js Route Handler Missing Error Handling

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.

The `bug.js` file contains code that attempts to retrieve a user from an array based on a user ID passed as a route parameter.  However, it fails to handle the case where the user ID is not a valid number, leading to potential crashes or unexpected behavior.

The `bugSolution.js` file provides a corrected version of the code, including robust error handling to address the issue.

## How to reproduce the bug

1. Clone the repository.
2. Run `npm install express` to install the required dependency.
3. Run `node bug.js`. 
4. Try accessing a route with an invalid user ID (e.g., `/users/abc`).

You'll observe an error (or unexpected behavior) due to the missing error handling.

## Solution

The solution involves adding input validation and handling the scenario where the user is not found, providing a more robust and user-friendly experience.