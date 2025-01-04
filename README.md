# CSS Hover Effect Propagation Bug

This repository demonstrates a common CSS bug where a hover effect unintentionally propagates to subsequent sibling elements. The problem lies in the use of the adjacent sibling combinator (`+`) in the hover selector.

## Bug Description
The `li:hover + li` selector unintentionally styles the list item immediately following the hovered item. This leads to unintended visual consequences and often makes the UI confusing for users. 

## Solution
The provided solution demonstrates how to avoid this unintended behavior by accurately selecting only the hovered list item.

## How to Reproduce
1. Open `bug.html` in your browser.
2. Hover over the list items. Notice how the next item also changes color.

## How to Fix
1.  Use the solution provided in `solution.css` which makes use of more appropriate selectors and isolates the styling to the current hovered list item.