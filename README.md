# React Router v6 - Incorrect Route Path Leading to 404

This example demonstrates a common issue in React Router v6 where a seemingly correct route path leads to a 404 error.

The problem arises from using an extension ('.html') in the route path that doesn't match the client-side URL.  While it may work in other frameworks, React Router by default ignores the extension. The solution is to remove it. 

## Bug
The `bug.js` file contains the buggy code.

## Solution
The `bugSolution.js` file demonstrates the corrected code. 

## How to reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`. 
4. Navigate to `/contact.html`. You'll encounter the 404 error.
5. Navigate to `/contact`. It will now work correctly.
