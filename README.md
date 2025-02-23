# React Router v6 - Unexpected Full Page Reload on Initial Route Transition

This repository demonstrates a bug in React Router v6 where an unexpected full page reload occurs during the initial transition between routes. Subsequent transitions to the same route work as expected.

## Bug Description

The application uses `react-router-dom` v6. When navigating from one route to another for the first time, a full page reload happens, unlike subsequent transitions which work correctly. This behavior isn't expected and disrupts the user experience.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate between the `/` and `/about` routes. Observe the full page reload on the first transition.

## Solution

The issue may be related to how the browser handles initial routing or interactions with other libraries or configurations. The solution involves ensuring that route changes are handled cleanly without forcing a full page reload.