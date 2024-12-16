# Uncommon HTML Bug: Hidden Div Still Affecting Layout

This repository demonstrates a subtle bug related to hiding HTML elements using CSS.  The incorrect use of the `visibility` property can lead to unexpected layout issues, even though the element appears hidden.

## Bug Description

The `bug.html` file contains a `div` element that is intended to be hidden. However, it uses the `visibility: hidden;` CSS property, which makes the element invisible but still retains its space in the layout.  This can cause problems with page flow and positioning of other elements.

The correct approach is to use `display: none;`, which removes the element from the layout entirely.

## Solution

The `bugSolution.html` file demonstrates the correct way to hide the element using the `display: none;` property. This resolves the layout issue and ensures the hidden element doesn't affect the rest of the page.

## How to reproduce

1. Clone the repository.
2. Open `bug.html` in a web browser. Observe that the div is invisible, but still affects the layout.
3. Open `bugSolution.html` to see the corrected version with the proper use of `display: none;`.