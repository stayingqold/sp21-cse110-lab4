## Part 1a
1. 20
2. 20
3. 20
4. This will return an error because `result` was created using let, so it is only available inside the if statement it was created in.
5. Line 7 will cause an error because `result` is constant. So we will not get to line 9.
6. Same thing as above, line 7 causes as error because `result` is a const. Even if there was no error in the if statement, it would not work because `result` is not in scope here.
 
## Part 1b
1. Line 12 will print out 3 because `i` is a `var`, so it stays in scope until the function ends.
2. Line 13 prints 150. In the last iteration of the for loop, we pass in 300, changing `discountedPrice` to be `300 * 0.5 = 150`. `discountedPrice` stays in scope because it is a `var`.
3. Line 14 prints 150. In the last iteration, `finalPrice` gets changed to `150 * 100 / 100 = 150`. `finalPrice` is a `var` so it is in scope.
4. This function will return `[50, 100, 150]`. We pass in `[100, 200, 300]`, and half each value and add it to `finalPrice`, then we return `finalPrice`.
5. We will get an error because `i` is now a `let` variable, so it is not defined on line 12.
6. We will get an error because `discountedPrice` is now a let variable, and we declared it inside the for loop, so we cannot access it outside the for loop.
7. Line 14 will print 150.
8. This function will return `[50, 100, 150]`. We pass in `[100, 200, 300]`, and half each value and add it to `finalPrice`, then we return `finalPrice`. `finalPrice` is declared outside the for loop as a `let` variable, so we can access it on line 16.
9. We will get an error because `i` is not defined in this scope.
10. Line 12 will print 3.
11. This function will return `[50, 100, 150]`. We pass in `[100, 200, 300]`, then half each one, then add it to `discounted`, which is what we return. `discounted` is a const variable, but we can still use the array it is assigned to. If we tried to assign it to a new array, it would cause problems.
12a. `student.name`
12b. `student['Grad Year']`
12c. `student.greeting()`
12d. `student['Favorite Teacher'].name`
12e. `student.courseLoad[0]`
13a. `'32'`: `2` is treated like a string
13b. `1`: `'3'` is treated like an integer
13c. `3`: `null` is treated like 0
13d. `'3null'`: `null` is treated like a string
13e. `4`: true is treated like the integer `1`
13f. `0`: `false` is treated like 0 and `null` is treated like 0.
13g. `'3undefined'`: undefined is treated like a string.
13h. `NaN`: It tries to do subtraction but does not work (undefined is not treated like 0, or like null)
14a. `true`: The string, `'2'`'s ascii value is higher than 1.
14b `false`: The ascii value for '2' is lower than that of '12'
14c. `true`: '==' is comparing the integer value 2 to the integer value in the string '2'
14d. `false`: '===' makes sure the two things being compared also have the same data type (which '2' and 2 don't)
14e. `false`: `true` is treat like 1, which is not equal to 2
14f. `true`: Anything other than an empty call, 0, -0, null, false, NaN, undefined, or the empty string makes the Boolean() call true. (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean). We then compare true to true which is true.
15. == first makes the two types being compared have the same value, then does the comparison. === first checks to make sure the items being compared have a similar type (so you can stil do 1.00 === 1), then compares them.
16. In part1b-question16.js
17. The result will be `[2, 4, 6]`. We pass `[1,2,3]` and `doSomething` into `modifyArray`. In `modifyArray`, we go through each item in `[1,2,3]` and create a new array with each value from `[1,2,3]` being modified by `callback`, which is `doSomething`. `doSomething` doubles the each value. We then return the new array that had every item doubled by `doSomething`.
18. in part1b-question18.js
19. The outpue it `1 \n 4 \n 3 \n 2`