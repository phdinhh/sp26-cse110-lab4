1. `3` is outputted at line 12. This is because `i` is the iterator for the previous `for` loop and `i` is declared with `var`. Therefore, as `i` is declared with `var`, `i` has no block scope and can be accessed even outside of the `for` loop.

2. `150` is outputted at line 13. This is because `discountedPrice` is declared with `var` and so `discountedPrice` has no block scope and can be accessed even outside of the `for` loop, even though `discountedPrice` was declared within the `for` loop. Therefore, `discountedPrice` would contain the last value of `discountedPrice` before the `for` loop ends.

3. `150` is outputted at line 14. This is because `finalPrice` is reassigned the discounted price of the last price of the array of `prices`. `finalPrice` is also declared with `var`, so it has no block scope and can be accessed within the function.

4. This function will return the array of discounted prices. In this case, the function will return `[50, 100, 150]` as `prices` is `[100, 200, 300]` and the `discount` is `0.5`. 

5. The code causes an error. This is because `i` is the iterator for the previous `for` loop and `i` is declared with `let` within that `for` loop. Therefore, as `i` is declared with `let`, `i` is only visible within the `for` loop code block, and the `console.log` at line 12 is outside the code block, and would not see `i`, which causes the error.

6. The code causes an error. This is because `discountedPrice` is declared with `let` within the previous `for` loop. Therefore, as `discountedPrice` is declared with `let`, `discountedPrice` is only visible within the `for` loop code block, and the `console.log` at line 13 is outside the code block, and would not see `discountedPrice`, which causes the error.

7. `150` is outputted at line 14. This is `finalPrice` was declared with `let` outside any other code block, so `finalPrice` is function-scoped and is visible to the `console.log` at line 14.

8. This function will return the array of discounted prices. In this case, the function will return `[50, 100, 150]` as `prices` is `[100, 200, 300]` and the `discount` is `0.5`. 

9. The code causes an error. This is because `i` is the iterator for the previous `for` loop and `i` is declared with `let` within that `for` loop. Therefore, as `i` is declared with `let`, `i` is only visible within the `for` loop code block, and the `console.log` at line 12 is outside the code block, and would not see `i`, which causes the error.

10. `3` is outputted at line 12. This is because `length` is the length of the `prices` array and `i` is declared with `const`outside any other code block, so `length` is function-scoped and is visible to the `console.log` at line 12.

11. This function will return the array of discounted prices. In this case, the function will return `[50, 100, 150]` as `prices` is `[100, 200, 300]` and the `discount` is `0.5`. Although `discounted` is declared with `const`, which means that `discounted` can't be reassigned with another value, the value within `discounted` can still be updated, so `discounted.push(discountedPrice)` doesn't cause an error as it only updates the value, rather than reassign.