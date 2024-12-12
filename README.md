# F# Mutable Variable Bug
This example demonstrates a potential issue when using mutable variables within F# functions.  The `add` function seems to correctly add `x` and `y`, but it might not behave as expected in more complex scenarios involving mutation inside the function. The solution demonstrates a more robust approach.

## Bug
The provided `bug.fs` file contains code illustrating unexpected behavior arising from modifying mutable variables within the function's scope. Specifically, the `add` function utilizes mutable variables, leading to issues that are harder to debug than an approach using immutable values.

## Solution
The solution is to refactor the code to use immutable values.   This improves the predictability and readability of the code and avoids potential side effects.