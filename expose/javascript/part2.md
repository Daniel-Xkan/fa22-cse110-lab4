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
13. A `32`, becuase 2 is automatically mapped to string '2'  B `1` becuase minus is arithmitic and string '3' auto converted to an int  C `3`, because null is auto convert into int 0 D `3null`, because null coverted to string null based on datatype of string '3' E `4`, because true is translated into int 1 and added to int 3. F `0`, because both false and null map to int 0 and 0 + 0 = 0  G `3undefined` because undefined is map to the string to match witht he type of string '3' H `NaN` because they are map to numbers in subtraction, but undefined cant map into numbers thus returning NaN. 
14. A `true` because string 2 mapped into int 2 and compared   B `false` because string comparasion is character by character, and 2 is larger than 1 thus false.  C `true`, string 2 mapped into int 2  D `false` because `===` stress the same type but they are different.  E `false` true mapped into int 1 != int 2  F `True`, because Boolean(2) return true, and true === true because of same type and value, thus return true.
15.  `==` will automatically do typecast, require same value but doesnt require same type. `===` require both the same value and same datatype. 
16.  see directory
17.  `[2,4,6]` will be returned. This is because the funciton `doSomething` is passed into the `modifyArray` function. `doSOmething` multiplies the number fo input parameter by 2. By passing `doSomething` in, the `modifyArray` use a for loop to pull out the input from old list and applied the function that doubles the number on each element of the list, and pushing them into a new list and return. Thus, 1,2,3 were pulled out and doubled one by one and pushed into new list to return, getting `[2,4,6]`.
18.  see directory
19.  `1 4 3 2` is the output. This is because the setTimeout doesnt wait for excuting the lines below, thus the print statement without setTimeout were printed then the setTimeout with less wait time is printed. 
<!-- 
Comparison
‘2’ > 1
‘2’ < ‘12’
2 == ‘2’
2 === ‘2’
true == 2
true === Boolean(2) -->