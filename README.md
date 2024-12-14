# React useEffect Hook Runs on Every Render

This repository demonstrates a common mistake when using the `useEffect` hook in React: forgetting to specify dependencies, causing it to run on every render instead of only when dependencies change.

## Problem
The `useEffect` hook in the provided `bug.js` file is defined without specifying the dependencies array.  This results in the effect running every time the component renders, leading to performance issues and unnecessary console logs.  This issue becomes more pronounced in complex components.

## Solution
The `bugSolution.js` file shows the corrected code.  The dependencies array `[count]` is added to the `useEffect` hook. This ensures the effect only runs when the `count` state variable changes.