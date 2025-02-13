# React Router v6 Catch-all Route Issue

This repository demonstrates a problem with catch-all routes ('*') in React Router v6.  The `NotFound` component, intended to handle all non-matching routes, does not render correctly.

## Problem

The provided code uses the `Routes` and `Route` components from `react-router-dom`. The catch-all route (`path="*"`) should render the `NotFound` component when accessing any route other than '/' and '/about'. However, it fails to do so.

## Solution

The solution involves ensuring that the catch-all route is positioned correctly in the `Routes` component.  It should be placed last to ensure all other routes are checked before it.  Additional considerations regarding nested routes and route order may need to be made based on the complexity of the app's routing structure.  This example shows a simple fix.