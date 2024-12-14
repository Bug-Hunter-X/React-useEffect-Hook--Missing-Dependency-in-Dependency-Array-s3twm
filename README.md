# React useEffect Hook: Missing Dependency in Dependency Array
This repository demonstrates a common React bug involving the useEffect hook and how to fix it.

## The Bug
The `bug.js` file contains a component that uses the `useEffect` hook to log the count. However, the dependency array is missing the `count` variable. This causes the effect to run on every render even when the count doesn't change, leading to excessive logging and potential performance issues.

## The Solution
The `bugSolution.js` file shows the corrected code. By including `count` in the dependency array, the effect now runs only when the `count` variable changes. This is the intended behavior and resolves the issue.

## How to reproduce
1. Clone this repo.
2. Navigate to the directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server. Observe the console logs. Compare bug.js and bugSolution.js to see the difference