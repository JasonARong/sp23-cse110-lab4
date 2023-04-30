# Part 1

1. 20
2. 20
3. 20
4. Error, because let variable result has block scope, it can only be accessed within the if statement. The second console.log on line 13 is outside of the if statement, so it cannot access the variable result.
5. Error, becuase const variable cannot be reassigned, but on line 5 it tried to reassign it with the sum of num1 and num 2
6. Error, same reason as 5. To reach line 13, `result = num1 + num2;` will be ran. Since reassigning const variable is prohibited, it will throw an error. And even if the reassigment does not happen, there still will be an error, because the const variable result is defined within the if statement, meaning it cannot be access outside of the if statement block scope.