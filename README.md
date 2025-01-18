# F# Mutable Variable Swap Bug

This repository demonstrates a common error when working with mutable variables in F#.  The `swap` function, intended to exchange the values of two mutable variables, unexpectedly modifies the original variables directly due to pass-by-reference semantics. The solution shows how to correctly swap values using a tuple or a different approach.

## Bug Description
The provided F# code attempts to swap the values of two mutable variables. However, because F# mutable variables are passed by reference, the swap function modifies the original variables instead of creating copies. This leads to both variables holding the same value after the `swap` function executes.

## Solution
The solution shows that the correct way to solve this issue is by either creating a copy of the values, working with tuples and immutable values, or using other mutable techniques.