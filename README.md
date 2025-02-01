# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: an infinite loop caused by a missing dependency in the `useEffect` hook.  The bug is described in detail below, along with a corrected solution.

## Bug Description

The `useEffect` hook is used to perform side effects after component rendering. If the dependency array is missing a value that changes on each render, the effect runs repeatedly, creating an infinite loop. This leads to performance degradation and potentially crashes.

## Solution

The solution involves adding the missing dependency to the useEffect dependency array.