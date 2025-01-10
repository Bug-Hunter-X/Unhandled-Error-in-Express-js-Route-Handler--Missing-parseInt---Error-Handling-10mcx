# Unhandled Error in Express.js Route Handler: Missing parseInt() Error Handling

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling when parsing user input.

The `bug.js` file shows the buggy code, which attempts to parse a user ID from the request parameters as an integer using `parseInt()` without checking for potential errors. If the `userId` is not a valid integer, this leads to a runtime error.

The `bugSolution.js` file provides a corrected version with improved error handling.  It uses a `try...catch` block to safely parse the user ID and handles cases where the ID is not found or is invalid.