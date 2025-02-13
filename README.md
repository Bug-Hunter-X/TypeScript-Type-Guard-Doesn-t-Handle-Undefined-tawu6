# TypeScript Type Guard Bug

This repository demonstrates a bug in TypeScript where a type guard that checks for null values doesn't correctly handle undefined values.  The function `greet` is designed to accept a string or null. However, when an undefined value is passed, TypeScript throws a type error.

## Bug Report

The provided `bug.ts` file contains a function `greet` that showcases this issue.  The function attempts to handle null values gracefully, but fails to consider the possibility of undefined.

The solution, found in `bugSolution.ts`, addresses this by explicitly checking for both null and undefined.