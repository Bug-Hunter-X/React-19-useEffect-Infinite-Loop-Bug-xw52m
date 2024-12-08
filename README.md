# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common bug in React 19 involving the `useEffect` hook, specifically an infinite loop caused by an incorrect dependency array.  The bug is triggered by an improper useEffect setup that causes a continuous re-render cycle.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders.  However, omitting or incorrectly specifying the dependency array causes unexpected behavior. This example demonstrates an infinite loop where the component continuously updates, leading to performance issues and potential crashes. The solution includes fixing the dependency array to only trigger the effect when the count variable changes.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install the required packages.
3. Run `npm start` to start the development server.
4. Observe the infinite loop in the browser's console.