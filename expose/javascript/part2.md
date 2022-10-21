# Part 2

## A Little MOre of a Challenge...
1. `3`, this is because the for loop in code stops at `i < prices.length`, and giving the length of price list is 3, at the last loop when i == 3, i < 3 was checked and exited
2. `150`, this is because discountPrice is declared as a variable that can be accessed outside the for loop, and the last loop stops at last element of List of Prices, which is 300 and the `discountPrice` is set to the value that cut its original price in half as shown: ` var discountedPrice = prices[i] * (1 - discount);` by the other input parameter `0.5`
3. `150`, 150 was the last variable in List, as talked above, the discountPrice is 150, thus final Price = `Math.round(150 * 100) / 100` = `150`
4. this function will return a List of discounted prices, namely `[50, 100, 150]`. THis is because we diffine the function to push input List element's discounted price into output list. 
5. `ReferenceError: i is not defined` error, this is because let variable was not accessible outside the loop by printing statment. 
6. `ReferenceError: discountedPrice is not defined at discountPrices`, since the local variable `discountPrice` declared by let cannot accessed outside its scope, its causing error on the printing statement. 
7. `150`, since the local variable `i` within loop was not accssed, but instead the finalPrice as discribed in previous problems, is printed. 
8. `[50, 100, 150]` will be returned similar to question4. There is no error because no one is calling on variable within the loop that used `let` to declare. 
9. `ReferenceError: i is not defined`. Error because i is only defined within the loop with `let` cannot access outisde loop.
10. `3`, because it will return the lenth defined by `const` on line 4 `const length = prices.length;`
11. `[50, 100, 150]`. This is because we are only assigning (pusing) values into the discounted list but not changing it, thus the `const` keyword will not generate error. 
12. A. student.name B. student['Grad Year'] C. student.greeting()  D. student['Favorite Teacher'].name E. student.courseLoad[0]
13. A '32', becuase 2 is automatically mapped to string '2  B  C D E F G H