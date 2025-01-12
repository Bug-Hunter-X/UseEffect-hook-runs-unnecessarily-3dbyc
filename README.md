# React useEffect Hook Unexpected Behavior

This repository demonstrates a common issue with the React `useEffect` hook where it runs even when a dependency array is specified, leading to unnecessary re-renders and potential performance problems. 

The `bug.js` file contains the problematic code. The `bugSolution.js` file provides the corrected version.

## Bug Description
The `useEffect` hook in the original code logs the current `count` to the console after every render.  Even though the dependency array `[count]` is provided, it still seems to run on every render. This is inefficient and can lead to unexpected side effects.

## Solution
The corrected code utilizes the dependency array correctly ensuring that the effect only runs when the count changes.  This is a more optimized and predictable approach.