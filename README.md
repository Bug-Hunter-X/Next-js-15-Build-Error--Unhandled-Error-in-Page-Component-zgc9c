# Next.js 15 Build Error: Unhandled Error in Page Component

This repository demonstrates a subtle build error that can occur in Next.js 15 when an unhandled error is thrown within a page component. The error is not caught during the build process leading to a failed build and potentially confusing error messages.

## Bug

The `pages/about.js` file throws an unhandled error.  In Next.js 15, this prevents the build from completing successfully.

## Solution

The solution involves implementing proper error handling.  This can involve using try...catch blocks or other error handling mechanisms.  Next.js 15 provides better error reporting in this situation, but unhandled errors in your page components still interrupt the build process. The example in `bugSolution.js` demonstrates a robust solution.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run build`.
4. Observe the build error.