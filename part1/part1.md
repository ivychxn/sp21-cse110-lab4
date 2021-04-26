## part 1a
1. values added: 20
2. final result: 20
3. values added: 20
4. error - result is declared in a different block, so it can't be accessed since we declared it with let
5. error - there's an attempt to reassign the variable on line 7. since it was declared with const, reassigning is not allowed.
6. error - same as the previous one. line 13 never executes because of line 7's error.

## part 1b
1. line 12 prints the variable i, which is 3. the variable i is used for the for loop to iterator to iterate through the prices array. the length of prices is 3, so i ends at 3.
2. line 13 prints the variable discountedPrice, which is just 150. since the for loop fully runs, discountedPrice is last value of the prices array multiplied by (1 - discount), which discount in this case is 0.5.
3. line 14 prints the variable finalPrice, which is 150. finalPrice is just the variable discountedPrice multiplied by 100 and rounded by Math.round, and then divided by 100. Math.round rounds to the nearest integer, and as shown in the last question, discountedPrice at the last iteration of the for loop is 150. 150*100 = 15000, and Math.round(15000) = 15000, and 15000/100 = 150 so finalPrice = 150
4. this function returns the discounted array, which is [50, 100, 150]. By the for loop, each value in the prices array is calculated with the discount, and then rounded to at most two decimals, and then put into the discounted array.
5. error - i is declared with let, but it's being referenced outside its scope since line 12  is not in the same block where it was initialized.
6. error - discountedPrice is declared with let, but it's being referenced outside its scope since line 13 is not in the same block where it was initialized.
7. line 14 will print 150, which is the value of finalPrice. line 14 is in the same block where finalPrice is declared with let, so there's no errors like the previous questions.
8. this returns the discounted array which is [50, 100, 150]. there's no issues with scope since line 16 is in the same block where discounted is declared with let.
9. error - line 11 is not within the block scope where i was declared with let.
10. line 12 prints 3. which is the length of the prices array.
11. The function will return the discounted array which is [50, 100, 150]. There's no issue with declaring discounted with const because there's no reassignment. We add values to the array by using push(), which isn't a reassignment.
12. 
* A. student.name
* B. student['Grad Year']
* C. student.greeting() 
* D. student['Favorite Teacher'].name 
* E. student.courseLoad[0]
13. 
* A. "32" since the 3 is a string so then 2 just appended to it
* B. 1 because the 3 is a stirng and can't be subtracted, so it turns into the numer 3, and then 3-2=1
* C. 3 since null becomes 0 and 3+0=3
* D. "3null" because null becomes the string "null" and is basically appended to the string "3" when added
* E. 4 since true becomes 1 and 3+1=4
* F. 0 since both false and null becomes 0 and 0+0=0
* G. "3undefined" because undefined becomes a string and is basically appended to the string "3" when added 
* H. NaN since undefined becomes NaN and any subtraction with that will just be NaN.
14. 
* A. true because '2' is converted to the number 2, which is greater than 1
* B. false because they're both strings and '2' > '1' (from '12') so the statement '2' < '12' is false
* C. true because '2' becomes the number 2, which is equal to 2
* D. false because different types cannot be compared and "===" means that there are no type conversions made in this case
* E. false because true becomes 1 so 1 == 2 is false
* F. true because Boolean(2) = true so even with the "===" comparing without type conversion, it doesn't make a difference since they're already the same type and value since true is equal to true
15. While they both check for equality, "==" allows for type conversions, but "===" compares without any type conversions
16. part1b-question16.js
17. The result is [2, 4, 6] because we're basically returning a new array where everything is doubled. We start with the array [1, 2, 3] and iterate through that with the for loop. For each element, the function doSomething doubles the value, and then that is pushed into the array newArr. As a result, we get [2, 4, 6] from [1, 2, 3]
18. part1b-question18.js
19. 1 4 3 2