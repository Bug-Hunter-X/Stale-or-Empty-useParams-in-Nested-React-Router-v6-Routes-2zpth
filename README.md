# React Router v6 useParams Issue in Nested Routes

This repository demonstrates a common problem encountered when using the `useParams` hook in deeply nested routes within React Router v6.  The issue revolves around the `useParams` hook not correctly updating with new parameter values when a parent route changes. This results in the `params` object being empty or containing outdated information.

## Problem Description

When navigating through nested routes, changes to parent route parameters may not automatically trigger re-renders in child components relying on `useParams`, leading to incorrect display of data.

## Solution

The provided solution uses the `useLocation` hook to trigger a re-render when necessary and ensures the correct parameters are retrieved and displayed.