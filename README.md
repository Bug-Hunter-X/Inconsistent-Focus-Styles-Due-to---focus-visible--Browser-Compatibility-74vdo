# Inconsistent Focus Styles Due to :focus-visible Browser Compatibility

This repository demonstrates a common CSS bug related to the `:focus-visible` pseudo-class and its lack of support in older browsers.  The bug results in inconsistent or missing focus styles for elements that should visually indicate focus.

## Bug Description
The `:focus-visible` pseudo-class provides a way to apply focus styles only when the focus is genuinely visible to the user (e.g., not triggered programmatically). However, older browsers don't support this pseudo-class, leading to a degraded experience for users of those browsers.

## Bug Reproduction
1. Open `bug.css` and `index.html` (this will be added).
2. Test in a modern browser (Chrome, Firefox, etc.) and an older browser (IE11, older versions of Safari).
3. Observe the inconsistent focus styles on the input field.

## Solution
The solution involves using a JavaScript polyfill for `:focus-visible` or providing alternative styling that works across all browsers. The `bugSolution.css` file shows one implementation.

## License
MIT