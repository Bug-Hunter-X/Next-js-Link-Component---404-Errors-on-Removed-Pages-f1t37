# Next.js Link Component - 404 Errors on Removed Pages

This repository demonstrates a potential issue with the Next.js `Link` component, where broken links might persist even after removing or renaming the target page.  This leads to 404 errors for users.

The `bug.js` file shows the problematic code.  The `bugSolution.js` file illustrates a better approach.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to the `/about` link.  This should work.
5. Remove the `pages/about.js` file.  The link will still be present but will result in a 404 error.  

## Solution

The recommended solution involves more robust error handling or a dynamic approach to generating links, as shown in the `bugSolution.js` file.