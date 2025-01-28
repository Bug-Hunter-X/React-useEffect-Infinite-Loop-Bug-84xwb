# React useEffect Infinite Loop Bug

This repository demonstrates a common issue with the React `useEffect` hook: an infinite loop caused by a missing dependency in the dependency array.

## Bug Description

The `useEffect` hook is designed to perform side effects after a component renders. However, if the dependency array is missing a value that changes during the render cycle, it leads to the effect constantly re-running, causing an infinite loop. This example illustrates such a scenario.

## Solution

The solution is simple. Ensure that all values used within the `useEffect` function are included in the dependency array.  This will prevent unnecessary re-renders and fix the infinite loop. 