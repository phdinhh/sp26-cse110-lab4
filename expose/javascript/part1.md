1. `values added:  20`

2. `final result: 20`

3. Because `var` has two main features, such as having no block scope and being able to be declared below their use, which may cause many issues with the `var` being hard to keep track of as well as debug when there are any issues.

4. `values added: 20`

5. The code returns an error because the variable `result` is declared within the `if` code-block. Therefore, as `result` is declared with `let`, `result` is only visible within that `if` code-block, and the `console.log` at line 13 is outside the code block, and would not see `result`, which causes the error.

6. The code returns an error because `result` is a `const`, which means that it cannot be reassigned. Therefore, when we try to reassign `num1 + num2` to `result`, an error is returned.

7. The code returns an error because `result` is a `const`, which means that it cannot be reassigned. Therefore, when we try to reassign `num1 + num2` to `result`, an error is returned.