# Unnecessary useEffect re-renders in React component

This repository demonstrates a common React bug where the `useEffect` hook is called after every render, even when it doesn't need to be. This can lead to performance issues and unnecessary console logs.

## Bug

The `bug.js` file contains a React component that uses the `useEffect` hook to log the current count to the console.  The problem is that this effect runs on every render. This is inefficient and can slow down the app for complex components. 

## Solution

The `bugSolution.js` file shows how to fix this bug using the optional dependency array in the `useEffect` hook. This ensures that the effect is only called when the count changes.

## How to reproduce

1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.