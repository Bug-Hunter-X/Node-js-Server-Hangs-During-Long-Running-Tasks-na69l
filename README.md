# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js where a server can hang or become unresponsive when performing long-running operations without proper asynchronous handling.  The `server.js` file contains the problematic code, while `serverSolution.js` shows how to fix it using asynchronous operations.

## Problem

The original `server.js` code simulates a long-running task within the main event loop. This blocks the event loop, preventing the server from processing new incoming requests.  This results in the server appearing to hang.