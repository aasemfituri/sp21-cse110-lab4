## Part 1a 
1. Line 9 prints "values added: 20"
2. Line 13 prints "final result: 20"
3. Line 9 prints "values added: 20" (assuming that line 13 would not give us an error)
4. Line 13 returns an error because we declared result using the "let" keyword and tried using the variable result outside of its scope (i.e outside of the if statement it was declared in)
5. The code returns an error because we cannot change "result" to num1 + num2 after it was initialize to 0.
6. Line 13 would also return an error because we used "const" to declare result and therefore we cannot access it outside of its scope.  

## Part 1b
1. Line 12 would print 3. The for loop would iterate 3 times (since the length of the array passed as an arugment is 3). i is incremented after each iteration, thus after the 3rd iteration we increment i to be 3 (from 2) and since the boolean condition (i < prices.length) is false we do not enter the for loop again and we simply print the value of i. The var keyword allows us the utilize the variable i anywhere within the function even if it is outside of the for loop.
2. Line 13 would print 150. In the final iteration of the for loop, discountedPrice gets the value of 300 * 0.5 = 150 and because discountedPrice is declared using the var keyword we can utilize it outside of the scope it was declared in, thus the line prints 150.  The var keyword allows us the utilize the variable discountedPrice anywhere within the function even if it is outside of the for loop.
3. Line 14 would print 150. In the last iteration of the for loop, we simply take the value of discountedPrice (which is 150 in this iteration) and multiply it by 100 (rounding) and then divide by 100. This effectively does nothing in this case and thus we return 150. Line 14 executes without any errors because finalPrice is still utilized within its scope (its declared at the beginning of the function).
4. This function will return an array of discounted prices, in which the prices are determined by the first argument and the discount is determined by the second argument. The for loop takes the prices of each element in the array and discounts them appropriately. Then the price is rounded and added to the array of discounted prices (discounted). In this specific example, the function would return [50,100,150] because the original array was [100,200,300] and the discount was 0.5 thus we reduce the price of every element in the array by 50%. The function returns without any errors because discounted is declared with the var keyword meaning that we can utilize it anywhere in the function.
5. The function returns an error at line 12 because we initialize i using the let keyword and thus it can be only accessed within the for loop. However, we are trying to access it outside of the for loop (outside of its scope).
6. The function will also return an error at line 13 for the same reason as above. We declared discountedPrices within the for loop using the let keyword and thus are only able to access it within the for loop. However, we try to access it outside of its scope and thus get an error.
7. Line 14 would print 150. This line does not return an error because we declared "final price" using the let keyword at the beginning of the function (outside of the for loop) and thus we can access it anywhere below its declaration within the function.
8. The function will return an array of prices that have been discounted. In this case it will return [50,100,150]. There is no error because the array discounted was declared outside of the for loop at the beginning of the function and thus can be used anywhere after its declaration in this function. For the logic of why the array returns discounted prices see (4) in part 1b.
9. The code would cause an error because we are trying to access the variable "i" outside of its scope (see (5)).
10. Line 12 would print 3. We declare length as the length of the prices array (which is 3) and thus print 3. No error occurs because we are still within the scope of the length variable (it was declared at the beginning of the function and thus we can utilize it anywhere after its declaration within the function).
11. The function will return an array of discounted prices which in this case is [50, 100, 150]. This does not cause an error even though discounted is declared using the const keyword and elements were added to the array because in this case const simply means that the value stored in discounted cannot change and that value is simply a memory address which we have not altered at all.  
12. A) student.name  
B) student["Grad Year"]  
C) student.greeting();  
D) student['Favorite Teacher'].name  
E) student.courseLoad[0]  
13.  A)'3' + 2 = 32  The 2 is converted to a string and the strings are concatenated.  
B)'3' - 2 = 1 The '3' is converted to an integer and the values are subtracted.  
C) 3 + null = 3 null is converted to the integer 0 and the values are added.  
D) '3' + null = 3null null is converted to the string "null" and the strings are concatenated.  
E) true + 3 = 4 true is converted to the integer 1 and the values are added.  
F) false + null = 0 false and null are both converted to the integer 0 and the values are added.  
G) '3' + undefined = 3undefined undefined is converted to the string "undefined" and the strings are concatenated.  
H) 3 - 'undefined' = NaN The string '3' is converted to the integer 3 and undefined is converted to NaN, thus subtracting them gives us NaN.  
14. A) '2' > 1 = true '2' is converted to the integer 2 and then compared to 1.  
B) '2' < '12' = false We simply compare the strings '2' and '12'. Thus, we first begin by comparing the first characters and since '2' comes after '1' the comparison evaluates to false.  
C) 2 == '2' is true. We convert '2' to the integer 2 and compare the two values.  
D) 2 === '2' is false. We first check if the values are of the same type and since they are not this evaluates to false.
E) true == 2 is false. true is converted to the integer 1 and then 1 is compared to 2.  
F) true === Boolean(2) is true. Boolean(2) evaluates to true and then we simply check if true === true and since they are the same type and same value the comparison evaluates to true.  
15) The == operator checks to see if two values are the same value after having performed the appropriate type conversions that JavaScript has. On the other hand === checks to see if two values are equal without converting any types.  
16) See [part1b-question16.js](part1b-question16.js)

17) The function will return a new array [2,4,6]. When we call modifyArray(), in each iteration of the for loop we call the callback function, which is doSomething. doSomething simply doubles the value of its argument, thus we simply double the value of each element in the array and push it into the new array.  
18) See [part1b-question18.js](part1b-question18.js)

19) The output of the code is:  
1  
4  
3  
2
