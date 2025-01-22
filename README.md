# React Native: Deprecated componentWillMount Lifecycle Method

This repository demonstrates a common issue in React Native applications: the use of the deprecated `componentWillMount` lifecycle method.  This method has been removed in recent versions of React Native and using it can lead to unexpected behavior or crashes.

The `bug.js` file shows the incorrect implementation using `componentWillMount`. The `bugSolution.js` file provides the corrected code using the appropriate lifecycle method or functional component approach.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run the application. You may observe unexpected behavior or a warning in the console.
4. Refer to `bugSolution.js` for the corrected implementation.

## Solution

The solution involves replacing `componentWillMount` with either:

* `componentDidMount` if you need to perform side effects after the component has mounted.
* A functional component with `useEffect` hook for cleaner, more modern code.