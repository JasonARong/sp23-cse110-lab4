# DevTools - Debugging
1. `.value` returns strings to both num1 and num2. So when `num1 + num2` executes, it will concatenate rather than additon.
2. Use built-in `number()` function to convert strings into numbers when initializing num1 and num2. [fix.png](./fix.png)