# Express.js - req.body is empty when receiving JSON POST request

This repository demonstrates a common issue in Express.js applications where `req.body` remains empty when receiving JSON POST requests.  The issue typically arises from a missing or incorrectly configured body-parsing middleware.  This example shows the problem and its solution.

## Bug
The `bug.js` file contains an Express.js server that attempts to process a JSON POST request. However, due to a missing middleware, `req.body` will be empty.

## Solution
The `bugSolution.js` file demonstrates the correct setup by including the `express.json()` middleware, which correctly parses the JSON request body. 

## How to run

1. Clone the repository.
2. Navigate to the repository directory.
3. Run `npm install` to install dependencies.
4. Run `node bug.js` to observe the incorrect behavior.
5. Run `node bugSolution.js` to see the corrected behavior.
