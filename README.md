# Unhandled Exception in Node.js HTTP Server

This repository demonstrates an uncommon error in Node.js where an unhandled exception within an HTTP request handler causes the server to crash without proper error logging or recovery.  The solution demonstrates best practices for handling exceptions and ensuring the server continues operation even in the face of errors.

## Bug

The `bug.js` file contains a Node.js HTTP server that throws an unhandled exception when a request is made to the `/error` endpoint. This causes the server process to terminate abruptly.

## Solution

The `bugSolution.js` file provides a solution by using a `try...catch` block to handle potential exceptions within the request handler.  This prevents the server from crashing and allows for appropriate error handling and logging.

The improved error handling ensures the server remains operational and provides informative error logs for easier debugging.