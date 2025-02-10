# React Native useRef Error: Cannot read properties of undefined (reading 'current')

This repository demonstrates a common error encountered when using the `useRef` hook in React Native:  "Cannot read properties of undefined (reading 'current')". This error occurs when accessing the `current` property of a ref before it has been assigned a value.  The provided code showcases the error and its solution.

**Problem:** The `useRef` hook's `current` property is initially `undefined`. Accessing it before the component has mounted or the ref has been assigned will throw this error.

**Solution:** Use a conditional check to ensure the ref has been assigned a value before attempting to access its `current` property. You can achieve this using the optional chaining operator (`?.`) or a simple `if` statement.