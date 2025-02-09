# React Native: undefined is not an object (evaluating 'this.state.myVar')

This repository demonstrates a common React Native error where attempting to access component state or props before the component has fully mounted results in an `undefined is not an object` error. The solution showcases how to properly access state and props within lifecycle methods.

## Problem

Accessing `this.state` or `this.props` within lifecycle methods like `componentDidMount` before the component has finished mounting leads to unexpected behavior and often the error `undefined is not an object (evaluating 'this.state.myVar')`.

## Solution

The solution uses the `useEffect` hook which allows for actions after the component mounts. This ensures `this.state` and `this.props` are properly defined before they are accessed.

## Usage

Clone the repository and run the provided code.  You can observe the error in `bug.js` and the solution in `bugSolution.js`.