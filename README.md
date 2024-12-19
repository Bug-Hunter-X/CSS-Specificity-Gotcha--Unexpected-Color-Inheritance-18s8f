# CSS Specificity Gotcha: Unexpected Color Inheritance

This repository demonstrates a subtle yet important CSS specificity issue. The problem arises from the interaction between selector specificity and the order of CSS rules.  Understanding how specificity works is crucial for avoiding unexpected styling behaviors.

## The Bug

The `bug.css` file contains CSS rules that seemingly conflict.  The expectation might be that the `<div class="special"></div>` element would be either blue (from the `div` rule) or red (from the `.special` rule), but this is incorrect.

The actual behavior is that the text color is green due to the specificity of the `.special div` selector.