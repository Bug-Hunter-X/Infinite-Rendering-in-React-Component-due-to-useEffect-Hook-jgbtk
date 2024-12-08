# Infinite Rendering Bug in React

This repository demonstrates a common React bug involving infinite rendering caused by a missing dependency array in the `useEffect` hook. The `useEffect` hook, without a dependency array, runs after every render, creating a loop.

## Bug Description

The `MyComponent` component uses `useState` to manage a count. The `useEffect` hook logs a message to the console after every render. Without a dependency array, the `useEffect` runs on every render, causing an infinite render loop.