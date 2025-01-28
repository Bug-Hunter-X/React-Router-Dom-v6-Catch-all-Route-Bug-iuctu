# React Router Dom v6 Catch-all Route Bug
This repository demonstrates a bug in React Router Dom v6 where the catch-all route (`*`) does not work as expected.  The issue arises when attempting to handle unmatched routes with a 404 page. The application displays a blank screen instead of the expected 404 page.

## Bug Description
The catch-all route, intended to catch all unmatched routes, fails to function correctly, leading to an unexpected blank screen.

## Solution
The solution involves ensuring that the catch-all route (`*`) is placed as the last route in the `Routes` component. This change correctly redirects unmatched routes to the 404 page. 

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to any unmatched route (e.g., `/invalid-route`).

You will observe a blank screen instead of the expected 404 page.

After applying the solution, repeat these steps.  The 404 page will now display correctly for unmatched routes.