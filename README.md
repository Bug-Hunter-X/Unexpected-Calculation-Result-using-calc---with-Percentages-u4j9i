# Unexpected Calculation Result using calc() with Percentages in CSS

This repository demonstrates a bug related to the unexpected calculation result when using the `calc()` function in CSS, specifically when combining percentages and other units. The calculated value deviates from the expected result.

## Bug Description
The `calc()` function is used to perform calculations within CSS. However, when combining percentages and other units (like pixels), the result might be incorrect.  This issue can lead to unexpected layout behaviors and visual discrepancies.

## Steps to Reproduce
1. Clone this repository.
2. Open `bug.css` and examine the `width` property of the `.box` element.
3. Notice the calculated width is not what you would expect based on a simple percentage calculation plus pixels.
4. Open `bugSolution.css` for a possible workaround.

## Possible Solution (see bugSolution.css)
In some cases, using only percentages or only fixed units might resolve the issue. Alternatively, ensure the order of operations within the `calc()` function is consistent and that the combined units are compatible.  Sometimes, using intermediate variables or a preprocessor can also help manage the complexity.