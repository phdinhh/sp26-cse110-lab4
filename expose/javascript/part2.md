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

12. 
A. `student.name`  
B. `student['Grad Year']`  
C. `student.greeting`  
D. `student['Favorite Teacher].name`  
E. `student.courseLoad[0]`  

13. 
A. `'32'` because integers map to their exact string representations  
B. `1` because strings are automatically converted to numbers in mathematical expressions  
C. `3` because null maps to 0 in numeric conversion  
D. `'3null'` because null becomes "null" when being concatanated with a string  
E. `4` because true maps to 1 in numeric conversion  
F. `0` because false maps to 0 and null maps to 0 in numeric conversion  
G. `'3undefined'` because undefined becomes "undefined" when being concatanated with a string  
H. `NaN` because undefined maps to NaN in numeric conversion  

14. 
A. `true` because string '2' becomes a number 2  
B. `false` because string '2' has higher dictionary order than '12'  
C. `true` because string '2' becomes a number 2  
D. `false` because number 2 and string '2' are not the same thing, as === is strict equality operator and there's no type conversion  
E. `false` because boolean true becomes a number 1  
F. `true` because Boolean(2) explicitly converts number 2 to a boolean true  

15. The == operator checks the equality after automatic type conversion, while === operator checks the equality without type conversion. In other words, with the == operator, two different types could still return true. Whereas, with the === operator, two different types would return false unless the values are explicitly converted to the same type.

16. Answer can be found in part2-question16.js

17. This function will return the array with all the values inside of it doubled. In this case, the function will return `[2, 4, 6]` as `array` was `[1, 2, 3]`. This is because for each value in `array`, the function `doSomething` is called on it (which doubles the input) and the result is pushed into `newArr`. Essentially, each value is updated to itself but doubled in this `newArr`, which is what the function returns.

18. Answer can be found in part2-question18.js

19. 
`1`  
`4`  
`3`  
`2`