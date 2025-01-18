# React Component Re-rendering Issue

This repository demonstrates a common issue in React applications where components fail to re-render when their state is an object or array.  This is due to React's shallow comparison of objects and arrays.

## Bug Description
The `bug.js` file shows a React component that uses `useState` to manage an object as its state. When updating the object, the component does not correctly re-render because the reference to the object remains the same. 

## Solution
The `bugSolution.js` file provides a fix using the `useMemo` hook to ensure that the component re-renders whenever the object's state changes.  This creates a new object reference upon state modification, triggering a re-render.

## How to run
1. Clone this repository.
2. Navigate to the repository's directory in your terminal.
3. Run `npm install` to install the necessary dependencies.
4. Run `npm start` to start the development server.