# React useEffect Hook Missing Dependency
This repository demonstrates a common bug in React applications involving the useEffect hook.  The issue arises from an incomplete dependency array, resulting in an infinite re-render loop.

## Bug Description
The `useEffect` hook is designed to perform side effects based on changes to specific values.  If a value that the effect depends on is not included in the dependency array, the effect will run on every render, leading to unexpected behavior and performance issues. This is especially problematic if the effect modifies state, leading to an infinite loop.

## Solution
The solution involves carefully reviewing the dependencies required by the `useEffect` hook and correctly including them in the dependency array.  This ensures the effect only runs when necessary.