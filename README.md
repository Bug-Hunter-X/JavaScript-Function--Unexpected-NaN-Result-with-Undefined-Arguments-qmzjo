# JavaScript Function: Unexpected NaN Result with Undefined Arguments

This repository demonstrates a common, yet subtle bug in JavaScript functions that can result in unexpected NaN (Not a Number) outputs. The bug arises from the function's failure to explicitly handle undefined values.

## The Bug

The `foo` function aims to add two numbers. It correctly handles null values by returning 0. However, it doesn't account for undefined values.  When an undefined value is passed as an argument, the addition operation results in NaN.

## The Solution

The solution involves explicitly checking for both null and undefined values, returning 0 in either case.