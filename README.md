# React useEffect Hook Missing Dependency Array

This repository demonstrates a common error in React applications: omitting the dependency array in the `useEffect` hook. This leads to unexpected behavior, such as infinite loops and performance problems.

## The Bug

The `bug.js` file contains a component that uses `useEffect` to update a counter every second. However, the dependency array is missing, causing the effect to run on every render, resulting in an infinite loop of counter increments.

## The Solution

The `bugSolution.js` file shows the corrected version with an empty dependency array (`[]`), causing the effect to run only once after the initial render. This is usually the preferred approach when the effect doesn't depend on props or state values.

## How to reproduce

1. Clone this repo
2. Run `npm install`
3. Run `npm start`
4. Observe the counter behavior in `bug.js` and `bugSolution.js`