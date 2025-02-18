# Missing Spaces in CSS calc() Function

This repository demonstrates a common error in CSS: forgetting spaces around operators within the `calc()` function. This can lead to unexpected results, such as elements not rendering correctly or having unexpected dimensions.

## The Bug

The incorrect code omits spaces, leading to parsing errors and unexpected behavior:

```css
/* Incorrect */
.element { width:calc(25%+10px); }
```

## The Solution

Adding spaces around the operators fixes the problem:

```css
/* Correct */
.element { width: calc(25% + 10px); }
```

Ensure to always include spaces around the `+`, `-`, `*`, and `/` operators in `calc()` to avoid this issue.