# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug causes an infinite loop due to an incorrectly specified dependency array.

## Bug Description
The `useEffect` hook is designed to perform side effects after every render. However, if the dependency array is not specified correctly, it can lead to unintended re-renders, causing an infinite loop. This example shows how omitting or incorrectly specifying dependencies can lead to this issue. 

## Solution
The solution involves correctly specifying the dependency array to prevent unnecessary re-renders.  By including only the necessary state variables in the dependency array, re-renders are triggered only when these variables change.