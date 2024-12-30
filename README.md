# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug is caused by an infinite loop due to a missing dependency in the `useEffect` hook's dependency array.  The solution demonstrates how adding the correct dependency resolves the problem.

## Bug
The `bug.js` file contains a component that uses the `useEffect` hook to log the current count. However, the effect has no dependency array, causing it to run on every render. This leads to an infinite loop.

## Solution
The `bugSolution.js` file corrects the bug by adding the `count` state variable to the dependency array. This ensures that the effect only runs when the `count` variable changes.