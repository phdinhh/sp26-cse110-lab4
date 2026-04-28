1. The bug is that `result` becomes the concatenation of `num1` and `num2`, rather than the addition of the two. This is apparent in the fact that `result` is of type `string` and is caused by the fact that `num1` and `num2` are strings, and so the `+` operator works as concatenation.

2. I would explicity type-cast each of `num1` and `num2` before addition.