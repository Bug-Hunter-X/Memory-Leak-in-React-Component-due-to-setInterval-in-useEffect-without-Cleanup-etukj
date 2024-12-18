# React UseEffect setInterval Cleanup Bug
This repository demonstrates a common bug in React applications: using `setInterval` within the `useEffect` hook without proper cleanup. This can lead to memory leaks and unexpected behavior.

## The Bug
The `bug.js` file contains a React component that uses `setInterval` to update a count every second. However, it fails to clear the interval when the component unmounts, resulting in a memory leak.

## The Solution
The `bugSolution.js` file provides a corrected version of the component. It uses the return value of `useEffect` to clear the interval when the component unmounts, preventing the memory leak.

## How to reproduce
1. Clone this repository
2. Run `npm install`
3. Run `npm start`