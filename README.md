# CSS Specificity and !important: An Unexpected Interaction

This repository demonstrates an uncommon bug related to CSS specificity and the `!important` flag.  The bug showcases a situation where a more specific CSS selector is unexpectedly overridden by a less specific selector because of the use of `!important`.

## Bug Description

A common assumption is that more specific CSS selectors will always override less specific ones. However, the `!important` flag can break this expectation, making debugging more challenging.  This example highlights this unexpected behavior.

## How to Reproduce

1.  Clone this repository.
2.  Open `bug.css` to see the problematic code.
3.  Open `bugSolution.css` to see the solution.

## Solution

The solution avoids using `!important` whenever possible and relies on proper CSS selector specificity to achieve the desired styling. Using `!important` should be considered a last resort due to its potential to create maintenance problems.