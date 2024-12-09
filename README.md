# Unhandled 'error' event in Node.js server

This repository demonstrates a common issue in Node.js servers: the lack of proper error handling, leading to unexpected crashes.

## Problem

The original `server.js` file contains a basic HTTP server.  However, it lacks a proper `'error'` event listener.  This means that if any error occurs (e.g., a network problem or an invalid request), the server will crash without providing useful information about the error.

## Solution

The `serverSolution.js` file demonstrates how to properly handle the `'error'` event using a listener. This allows for graceful handling of errors, preventing unexpected server crashes, and providing more details for debugging.

## How to run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/nodejs-error-handling.git
   ```
2. Navigate to the directory:
   ```bash
   cd nodejs-error-handling
   ```
3. Run the original (buggy) server (optional):
   ```bash
   node server.js
   ```
4. Run the fixed server:
   ```bash
   node serverSolution.js
   ```

Try to make requests to both servers to observe the difference in error handling.