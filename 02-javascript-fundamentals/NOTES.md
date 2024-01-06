# JavaScript Fundamentals


- use the console.log command to print out messages
- use double slashes (//) to write code comments
- use forward slash (/) and an asterisk (*) to write multi-line comments

## Number Data Type

### Relative comparison operators

- `>` (greater than)
- `<` (less than)
- `>=` (greater than or equal to)
- `<=` (less than or equal to)
- `===` (equal to)
- `!==` (not equal to)


## Boolean Data Type

### Logical Operators


- `!` (not)
- `&&` (and)
- `||` (or)

### De Morgan's Law

A common mistake in boolean logic is to incorrectly distribute ! across parentheses. Say we had boolean values of A, B. Here is something to remember:

- `!(A || B)` is equivalent to `!A && !B`
- `!(A && B) `is equivalent to `!A || !B`


## String Data Type

- a String is a data type that contains multiple characters enclosed in quotation marks
- `string.length` returns the number of characters in the string
- each character of a string is associated with a numerical index; the first character of a string is at index 0
- we can use `string.indexOf(char)` to obtain the index of char within string; if char is not found, then -1 is returned
- we can use `+` to concatenate multiple strings, combining them into a single string
- use backticks `\`` to create template literals

## Array Data Type

- An Array is a data type that contains a list of in order values surrounded in square brackets `[]`.
`array.length` returns the number of values in the array.
- Each value of an array is associated with a numerical index; the first value of an array is at the index of 0.
- We can use `array.indexOf(value)` to obtain the index of value within array; if value is not found, then -1 is returned.
- We can use .`concat` to concatenate multiple arrays, combining them into a single array.


### Template Literal

```javascript
let string = `Let me tell you ${1 + 1} things!`;
console.log(string); // Let me tell you 2 things!
```

## Conditionals

- Conditional statements allow us to control what actions should be taken based on a boolean (truthy or falsey) expression
- In a chain of then expressions (`if...else if...else`), only one of the then expressions will be executed.
- Conditional statements can have only one `if` and one `else` statement.
- Conditional statements can be nested.


## Loops

```javascript
// these two do the exact same thing!
function forLoopDoubler (array) {
  // it is convention to shorten index to just i in most cases
  for (let i = 0; i < array.length; i++) {
    array[i] = array[i] * 2;
  }
  return array;
};

function whileLoopDoubler (array) {
  let i = 0;
  while (i < array.length) {
    array[i] = array[i] * 2;
    i++;
  }
  return array;
};

forLoopDoubler([1, 2, 3]); // => [2,4,6]
whileLoopDoubler([1, 2, 3]); //=> [2,4,6]
```
