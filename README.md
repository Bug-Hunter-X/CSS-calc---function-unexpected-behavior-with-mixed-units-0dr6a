# CSS `calc()` Function Unexpected Behavior with Mixed Units

This repository demonstrates a subtle bug in the CSS `calc()` function related to unexpected behavior when combining different units (like `vw`, `vh`, `px`, percentages), and particularly concerning the order of operations and the timing of percentage calculations.

## Problem

The `calc()` function sometimes produces unexpected results when used with multiple units or a mix of units and percentages, due to the order of operations and the timing of percentage calculation. The behavior may be inconsistent across different browsers or depend on other factors, leading to layout inconsistencies.

## Solution

The solution involves careful consideration of the units being used and ensuring the correct order of operations.  In some cases, it may be necessary to use intermediate variables or helper classes to simplify the calculation. Also, making sure the percentage is calculated from an already rendered parent container is also important.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` and `bugSolution.css` to see the buggy and fixed versions, respectively.
3. Observe the differences in the rendered output.