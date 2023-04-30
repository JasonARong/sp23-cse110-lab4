# Part 2

1.  It will log out 3. Because variable i will be incremented 3 times in the for loop, as the input array "prices" has a length of 3. Moreover, vairable i is decleared as a var, meaning it has function scope. So it can be logged out on line 12, even it is outside the for loop.
2.  It will log out 150. Because if var variables have same name, the lastest declare variable will overwrite the ones that are declared ealier. So in the final iteration of the for loop var discountedPrice will be set to 150 and overwrite the previous discountedPrice declared in ealier loop iteration. And since it is var, it can be log out on line 12 which is outside the for loop block.
3.  It will log out 150. finalPrice is declare under the function discountPrices as a var varible, so it can be accessed anywhere inside the function. The for loop, therefore, can access it and update it. In the final iteration of the for loop, since the discountedPrice will be set to 150, the finalPrice will be updated to be 150 as well. Hence, 150 will be logged out on line 14.
4.  It will return [50, 100, 150]. The function discountPrices takes in an array of [100, 200, 300] as prices, and a number 0.5 as discount. It first initializes an empty array discounted, and set a varaible finalPrice to be 0. And then it starts a for loop that the number of iteration is the same as the length of the prices array which is 3. The for loop iterates over each item in the prices array using the index variable i. For each interation, a var variable discountedPrice will be declared and set to discounted price of each item by multiplying the original price with `1 - discount`. The finalPrice will then be updated by round the value of discountedPrice to 2 decimal places. After that, the finalPrice of its corresponding original value will be appended to the discounted array. Since the input value for discount is 0.5, a 50% of discount will be applied to each item of the prices array. Therefore, the result will be [50, 100, 150].
5.  Error. Because the let variable i is declared in the for loop. Since let only has block scope and the console.log on line 12 is outside of the for loop block, it cannot access the let i variable.
6.  Error. Because the let variable discountedPrice is declared in the for loop. Since let only has block scope and the console.log on line 13 is outside of the for loop block, it cannot access the let discountedPrice variable.
7.  It will log out 150. The let variable finalPrice is declared inside the discountPrices function block. Since the for loop and the console.log are both encapsulated by the function block, both can access the finalPrice variable. And after teh final iteration of the for loop discountPrices will be updated to be 150. Hence, 150 will be logged out.
8.  It will return [50, 100, 150]. The reason why it works is similar to #4, as the discountPrices function takes in an array of [100, 200, 300] as prices, and a number 0.5 as discount. It loops over all the values in the array and discount each of them by 50% and append to the discounted array and return. The main difference is how dicountedPrice works under the hood. Within each loop, a new block scope is created for each iteration. And since let variable has block scope, dicountedPrice declared using let within the loop can be declared multiple times. Therefore, it returns the correct result.
9.  Error. Because the let variable i is declared in the for loop. Since let only has block scope and the console.log on line 11 is outside of the for loop block, it cannot access the let i variable.
10. It will log out 3. On line 4 const variable length is  declared under the block scope of the function discountPrices and set to the length of array prices which is 3. Const has block scope, the console.log on line 12 is also under the discountPrices function's block scope, so it can successfully log out lenth's value which is 3.
11.  It will return [50, 100, 150]. The function discountPrices takes in an array of [100, 200, 300] as prices, and a number 0.5 as discount. It first initializes an empty array discounted, and set a const varaible length to be the length of the input array prices which is 3. And then it starts a for loop that iterates over each item in the prices array using the index variable i. For each interation, a new block scope will be created. Within each loop block, a const variable discountedPrice will be declared and set to discounted price which is 50% of its original value, since the discount value is 0.5. After that, the finalPrice of its corresponding original value will be appended to the discounted array. Even though the discounted array is declared by const, its value can be modified (but reassigment is not allowed). As a result, after the for loop, the content of the discounted array will be [50, 100, 150].
12. Data Types
    1. student.name;
    2. student['Grad Year'];
    3. student.greating();
    4. student['Favorit Teacher'].name;
    5. student.courseLoad[0];
13. Arithmetic
    1. 32
    2. 1
    3. 3
    4. 3null
    5. 4
    6. 0 ?
    7. 3undefined
    8. NaN
14. Comparison
    1.  true
    2.  true
    3.  true
    4.  false
    5.  false
    6.  true
15. The difference between the == and === operators is that == does the type conversion of the operands before comparison, but === compares the values as well as the data types of the operands.
16. [part2-queation16.js](./part2-question16.js)
17. The result will be [2, 4, 6]. On line 13, modifyArray function is called. It was called with 2 arguments: an array of [1, 2, 3] and a callback function doSomthing. Inside the modifyArray function, it first creates an empty newArr array. And then, it iterates over the original array [1, 2, 3] using a for loop. For each element of the original array, it is used as an  argument to call the callback function doSomthing. And inside the callback function doSomthing, it will return 2 times the value of whatever is passed in. After the doSomthing returns, the result will be pushed into newArr. After, the loop finished iterating over the 3 numbers in the orginal array, the for loop terminates, and the modifyArray function returns newArry which has the value of [2, 4, 6].
18. [part2-question18.js](./part2-question18.js)
19. 1,4,3,2