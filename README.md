# CSS :nth-child Unexpected Behavior with Negative Index

This repository demonstrates a subtle bug related to the unexpected behavior of the CSS `:nth-child` pseudo-class when using a formula that results in a negative index.  The provided CSS code uses the formula `-n + 1`, which produces negative indices for values of `n` greater than 1. The expected behavior isn't clearly defined by the specification for these cases, leading to inconsistent rendering across browsers.

The `bug.css` file contains the erroneous CSS, while `bugSolution.css` provides a corrected approach.  This example highlights the importance of carefully crafting `:nth-child` selectors to avoid unexpected behavior and ensure consistent styling across different browsers and environments.

## Issue

The `-n+1` formula in `:nth-child` does not work as expected for `n` values greater than one. It doesn't seem to select the elements in the intended manner. This inconsistency leads to unexpected visual results and makes the CSS less reliable.

## Solution

The solution involves using an appropriate selector that correctly targets the desired elements.  This might involve rewriting the selector entirely or employing a different CSS technique to achieve the same styling results.