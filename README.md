# React Router DOM Catch-All Route Issue

This repository demonstrates an unexpected behavior with catch-all routes (`/*`) in React Router DOM v6.  The catch-all route doesn't behave as expected, showing the 404 page even for valid paths.

## Problem

The provided `App.js` demonstrates a simple React Router setup.  Despite having routes defined for `/` and `/about`, the catch-all route `/` always seems to be triggered. 

## Solution

The solution, `AppSolution.js`, demonstrates that the `/*` route should be placed last to ensure it only catches routes not matched by other routes. 