# CSS :nth-child Dynamic Update Issue

This repository demonstrates a common issue with the CSS `:nth-child` selector: it doesn't automatically update when elements are added or removed to the DOM after the page has initially loaded.

## Problem

The `:nth-child` selector is evaluated only once during initial page rendering. If you dynamically modify the DOM (e.g., adding or removing list items via JavaScript), the styling applied by `:nth-child` won't reflect those changes. This often leads to inconsistent or unexpected visual results.

## Solution

The solution involves using JavaScript to re-apply the styles after the DOM has changed. This typically involves querying the relevant elements and updating their styles.  A more robust solution may also involve using JavaScript frameworks or libraries that manage DOM updates more efficiently.