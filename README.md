# React useEffect Hook Missing Dependency

This repository demonstrates a common error in React's `useEffect` hook: a missing dependency.  The `useEffect` hook is intended to perform side effects, but if dependencies aren't correctly specified, side effects may not occur as expected, or they might occur at unexpected times.

The example shows a `MyComponent` that updates a counter.  An `useEffect` hook is used to log a message when the `count` exceeds 5.  However, because the dependency array is empty, the `if` condition within `useEffect` is only evaluated once, during the initial mount. This means the message will only log once, even if `count` later exceeds 5.  The solution demonstrates how to fix this issue.
