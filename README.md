# Uncommon HTML Error: Using Number in innerHTML

This repository demonstrates an uncommon error that can occur in HTML when using the `innerHTML` property with a number instead of a string.  Some browsers might not explicitly throw an error but can result in unexpected output or behavior. This example showcases the issue and its solution.

## Bug Description

The `innerHTML` property of a DOM element is designed to work with strings.  Attempting to assign a number directly to it might lead to inconsistent rendering or silent failures.  Not all browsers handle this consistently, making it an easily overlooked and potentially difficult to debug issue.

## How to Reproduce

1. Open `bug.html` in your web browser.
2. Observe the content within the `div` element. The number 123 will be rendered but there might be errors or unexpected behavior.

## Solution

The solution is straightforward: ensure you assign a string to `innerHTML`.  If you're working with numbers, convert them to strings using `toString()` before using them with `innerHTML`.

Open `bugSolution.html` to see the corrected code.