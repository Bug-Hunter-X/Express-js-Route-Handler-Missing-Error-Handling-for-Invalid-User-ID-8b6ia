# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  Specifically, the `/users/:id` route attempts to parse the `id` parameter as an integer without handling potential errors if the `id` is not a number.

## Bug

The `bug.js` file contains the flawed code.  It attempts to find a user based on their ID, but if the `id` is not a valid integer or the user is not found, it will throw an error.

## Solution

The `bugSolution.js` file provides a corrected version of the code.  It includes comprehensive error handling to check if the `userId` is a number and handle the case where the user is not found gracefully.