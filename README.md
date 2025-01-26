# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript error related to loose equality (==) when handling null and undefined values.  The `bug.js` file contains code that showcases the unexpected behavior. The `bugSolution.js` file offers a solution using strict equality (===) to improve code reliability.

## Problem

JavaScript's loose equality operator (==) performs type coercion, which can lead to unexpected results when comparing null and undefined. In this case, null == undefined evaluates to true, which can lead to logical errors in applications.

## Solution

The preferred solution is to use the strict equality operator (===), which does not perform type coercion. This ensures that comparisons are precise and avoid the unexpected behavior caused by loose equality.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and observe the output. Note the unexpected NaN value returned when passing undefined. 
3. Open `bugSolution.js` to see the corrected code that correctly handles both null and undefined cases using strict equality.
