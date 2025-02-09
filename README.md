# React Router v6 Nested Route Conflict with Wildcard Route

This repository demonstrates a common issue encountered when using nested routes with a wildcard route ('/*') in React Router v6.  The wildcard route, intended to catch 404 errors, can inadvertently prevent nested routes from rendering correctly.

## Problem
The problem arises when a parent route's path overlaps with or is more general than a child route's path and a wildcard route is present.  The wildcard route will always match first, regardless of more specific child routes.

## Solution
The solution involves carefully ordering routes and potentially using an index route to manage the 404 case effectively, while enabling nested route functionality without conflict.  This example shows how to avoid the issue by prioritizing more specific path matching before the wildcard route.

## Setup
1. Clone this repository.
2. Navigate to the project directory `cd react-router-v6-issue`
3. Install dependencies `npm install`
4. Run the application `npm start`
