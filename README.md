# Unhandled Exception in Asynchronous Callback in Node.js

This repository demonstrates a common error in Node.js applications: unhandled exceptions within asynchronous callbacks.  Improper error handling in asynchronous code can lead to crashes and unexpected behavior.

## The Problem

The `bug.js` file contains a simple Express.js server.  It simulates an asynchronous operation using `setTimeout`.  There's a 50% chance an error is thrown within the callback. Without proper error handling, this error will crash the server.

## The Solution

The `bugSolution.js` file demonstrates the correct approach: using `try...catch` blocks within asynchronous callbacks or utilizing appropriate middleware to handle errors gracefully.