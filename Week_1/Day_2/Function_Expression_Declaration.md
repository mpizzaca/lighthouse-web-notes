# Function Declaration vs Expression

### Function Declaration
```javascript
function someFunction() {

}
```
- hoisted (ie. can call the function above its declaration)
- can overwrite previously declared functions (the last one will be hoisted and called throughout the file)

### Function expression
```javascript
const someOtherFunction = function() {

}
```
- not hoisted (ie. cannot call the function above it's declaration)
- will throw a SyntaxError if you try to overwrite the function expression or a TypeError if you try to reassign the const variable to a new function


## Summary
- Should always use Function Expressions, with the exception of exporting functions in React (as you can use `export default` in one line with Function Declarations only)