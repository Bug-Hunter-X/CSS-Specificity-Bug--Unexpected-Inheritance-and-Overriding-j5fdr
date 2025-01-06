# CSS Specificity Bug: Unexpected Inheritance and Overriding

This repository demonstrates a subtle bug related to CSS specificity and inheritance.  The issue involves a more specific selector (`div p`) being unexpectedly overridden by a less specific one (`div`).

## Bug Description

A `div` element has a blue color, and a `p` element within that `div` should have a green color due to the more specific rule (`div p`). However, in certain browsers or contexts, the `p` element may inherit the color from the parent `div`, resulting in blue text, rather than green.

## Solution

The solution involves adjusting the specificity of the CSS rule so that `div p` always takes precedence. More details in `bugSolution.css`.