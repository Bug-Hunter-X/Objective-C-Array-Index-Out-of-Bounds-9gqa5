# Objective-C Array Index Out of Bounds Error

This repository demonstrates a common Objective-C error: accessing an array element using an index that's out of bounds.  The code attempts to iterate beyond the valid index range of an array, which can lead to crashes or unexpected behavior.

## The Bug
The bug lies in the loop's condition.  It should iterate up to, but not including, `myArray.count`. Incorrectly, it iterates one element past the valid range.

## The Solution
The solution corrects the loop condition to ensure the index stays within the bounds of the array.

## How to reproduce the bug
1. Clone this repository.
2. Compile and run the code.
3. Observe the crash or unexpected output.

## How to fix the bug
1. Replace the loop condition `i <= myArray.count` with `i < myArray.count`.
2. Recompile and run the code. 