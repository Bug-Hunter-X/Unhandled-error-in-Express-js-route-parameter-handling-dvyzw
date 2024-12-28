# Express.js Route Parameter Handling Bug

This repository demonstrates a common error in Express.js applications when handling route parameters. The bug occurs when trying to access a parameter before ensuring the data associated with the parameter exists, leading to an error if the data is not found.

## Bug Description

The `bug.js` file contains code that attempts to access a user from a database based on an ID passed in the route parameter.  If the user with the given ID does not exist, the code throws an error because it tries to access a non-existent variable.

## Solution

The `bugSolution.js` file provides a corrected version of the code. It first checks if the user exists before attempting to access its properties. This prevents errors when a user with the specified ID is not found.