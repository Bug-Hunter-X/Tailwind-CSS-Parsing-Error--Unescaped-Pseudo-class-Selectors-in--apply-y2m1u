# Tailwind CSS Parsing Error: Unescaped Pseudo-class Selectors in @apply

This repository demonstrates a common error encountered when using Tailwind CSS's `@apply` directive with pseudo-class selectors. The error arises from incorrectly using pseudo-class selectors within the `@apply` directive, causing a parsing failure by the Tailwind compiler.

## Problem
The core issue is a conflict between Tailwind's class naming conventions and the presence of colons (`:`) in pseudo-class selectors such as `:hover`, `:focus`, etc.  Directly using such selectors within `@apply` can lead to parsing errors.

## Solution
The correct approach is to use the utility classes directly or to create a custom class containing the desired styling for better maintainability and cleaner code.  This ensures Tailwind correctly processes the directives and avoids any conflicts.

## How to reproduce
1. Clone this repository.
2. Examine `bug.css` to see an example of the incorrect usage.
3. Observe the compilation error (or lack thereof).
4. Examine `bugSolution.css` to see the correct usage. 
5. Test the corrected code and the bug.

