# Unhandled Promise Rejection in Express.js Server

This example demonstrates a common error in Node.js Express.js servers: unhandled promise rejections.  The server starts and appears to function, but if the asynchronous operation (`someAsyncOperation`) fails, the error is silently swallowed, leaving the client with no response and the server continuing to run. 

The `bug.js` file shows the problematic code.  The solution, in `bugSolution.js`, demonstrates the correct way to handle potential errors within asynchronous operations and respond appropriately to the client.