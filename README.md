# Node.js Server Unresponsiveness

This repository demonstrates a common Node.js issue: server unresponsiveness caused by a long-running synchronous operation within the request handler.  The `server.js` file contains the problematic code, which simulates a 5-second delay.  This blocks the event loop, preventing the server from responding to subsequent requests.

The `serverSolution.js` file shows how to resolve this by using asynchronous operations or offloading the long-running task to a worker thread or separate process.