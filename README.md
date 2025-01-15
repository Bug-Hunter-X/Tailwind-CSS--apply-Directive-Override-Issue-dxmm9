# Tailwind CSS @apply Directive Override Issue

This repository demonstrates an uncommon bug related to the `@apply` directive in Tailwind CSS.  The issue occurs when custom CSS classes containing properties that also exist in Tailwind's default styles are applied using `@apply`.  Tailwind's defaults will override the custom styles despite order or specificity.

## Steps to Reproduce

1. Clone this repository.
2. Open `bug.css` and `bugSolution.css` to see the buggy and corrected code.
3. Observe how `bg-blue-500` overrides the `background-color: #ff0000` in the buggy example.

## Solution

The solution involves using utility-first approach or ensuring that your custom styles are more specific and avoid naming conflicts with Tailwind utilities.