# React useEffect setInterval Memory Leak
This repository demonstrates a common error in React applications involving the use of `setInterval` within the `useEffect` hook and its solution.

## Problem
The `setInterval` function, when used without proper cleanup within `useEffect`, creates a memory leak and continues running even after the component is unmounted. This leads to performance degradation and potential unexpected behavior.

## Solution
The provided solution illustrates the correct usage of `setInterval` within `useEffect` by adding a cleanup function using the `return` statement. This cleanup function ensures the interval is cleared when the component is unmounted preventing the memory leak.

## How to run:
1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.