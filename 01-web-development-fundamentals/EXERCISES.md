# Web Development Fundamentals

## JavaScript Fundamentals

### Hello World REPL

```javascript
console.log("Hello World!");
```

### Numbers Exercise

```javascript
// Example:
console.log(4 + 2.5)   // 6.5

// Write 5 more expressions below:
console.log(1 + 1); // 2
console.log(1 - 1); // 0
console.log(1 * 1); // 1
console.log(1 / 1); // 1
console.log(1 % 1); // 0
```

### Boolean Exercise

```javascript
// Example:
console.log(false || false)   // false

// Write 3 more expressions below:
console.log(!true); // false
console.log(true && false); // false
console.log(true || false); // true
```

### Goodbye

```javascript
function goodbye(name) {
  return "Bye " + name + ".";
}

console.log(goodbye("Daniel")); // => "Bye Daniel."
console.log(goodbye("Mark")); // => "Bye Mark."
console.log(goodbye("Beyonce")); // => "Bye Beyonce."
```

### Muscle Memory
Note: I got sick of making functions so I just made one with multiple parameters so I could call it with different arguments for variety.

```javascript
function sayHello(name) {
  let msg = "Hello, " + name + ". How are you?";
  return msg;
}

function sayGoodbye(name) {
    return "Goodbye, " + name + ".";
}

function say(word, name) {
    return word + ", " + name + ".";
}

console.log(sayHello("world"));
console.log(sayGoodbye("world"));
console.log(say("Hello", "world"));
console.log(say("Hi", "world"));
console.log(say("Goodbye", "world"));
console.log(say("Bye", "world"));
console.log(say("Cheerio", "world"));
console.log(say("Greetings", "world"));
console.log(say("Bonjour", "world"));
console.log(say("Ciao", "world"));
```


### Plus 5

```javascript
function plusFive(num) {
  return num + 5;
}

console.log(plusFive(10));  // => 15
console.log(plusFive(2));   // => 7
console.log(plusFive(-8));  // => -3
```

### Call This Function

```javascript
function isCool(string) {
  let coolSentence = string + " is cool!"
  console.log(coolSentence)
  return coolSentence
}

// Call the above function passing in the below arguments:
// Music
// JavaScript
// The world
isCool("Music");
isCool("JavaScript");
isCool("The world");
```

### Average of Two

```javascript
function averageOfTwo(num1, num2) {
  return (num1 + num2) / 2;
}

console.log(averageOfTwo(3, 7)); // => 5.0
console.log(averageOfTwo(16, 5)); // => 10.5
console.log(averageOfTwo(2, 7.5)); // => 4.75
```

### Hello

```javascript
function hello(str) {
  console.log("Hello, " + str);
}

hello("cat"); // prints "Hello, cat"
hello("Helen"); // prints "Hello, Helen"
hello("Sting"); // prints "Hello, Sting"
```

### Divide by Three

```javascript
function divideByThree(num) {
  return num / 3;
}

console.log(divideByThree(9)); // => 3.0
console.log(divideByThree(15)); // => 5.0
console.log(divideByThree(98)); // => 32.666666666666664
```

### Whisper

```javascript
function whisper(str) {
  return "..." + str.toLowerCase() + "...";
}

console.log(whisper("Hey Buddy")); // => "...hey buddy..."
console.log(whisper("YEA! that was fun")); // => "...yea! that was fun..."
```

### Average of Four

```javascript
function averageOfFour(num1, num2, num3, num4) {
    return (num1 + num2 + num3 + num4) / 4;
}

console.log(averageOfFour(10, 10, 15, 5)); // => 10
console.log(averageOfFour(3, 10, 11, 4)); // => 7
console.log(averageOfFour(1, 2, 3, 4)); // => 2.5
```

### Yell

```javascript
function yell(str) {
  return str.toUpperCase() + "!!!";
}

console.log(yell("I want to go to the store")); // => "I WANT TO GO TO THE STORE!!!"
console.log(yell("Time to program")); // => "TIME TO PROGRAM!!!"
```

### Echo

```javascript
function echo(string) {
  let result = string.toUpperCase() + " ... ";
  result += string + " ...";
  result += string.toLowerCase();
  console.log(result);
  return result;
}

echo("Mom!"); // => prints "MOM! ... Mom! ... mom!"
echo("hey"); // => prints "HEY ... hey ... hey"
echo("JUMp"); // => prints "JUMP ... JUMp ... jump"
```

### Is Five

```javascript
function isFive(num) {
    return num == 5;
}

console.log(isFive(5)); // => true
console.log(isFive(13)); // => false
```

### Is Odd

```javascript
function isOdd(num) {
  return num % 2 !== 0;
}

console.log(isOdd(2)); // => false
console.log(isOdd(5)); // => true
console.log(isOdd(-17)); // => true
```

### Is Substring

```javascript
function isSubstring(searchString, subString) {
  const searchLower = searchString.toLowerCase();
  const subLower = subString.toLowerCase();
  return searchLower.indexOf(subLower) !== -1;
}

console.log(isSubstring("The cat went to the store", "he cat went")); // => true
console.log(isSubstring("Time to program", "time")); // => true
console.log(isSubstring("Jump for joy", "joys")); // => false
```

### Log Between

```javascript
function logBetween(lowNum, highNum) {
    for (let i = lowNum; i <= highNum; i++) {
        console.log(i);
    }
}

// Examples:
logBetween(-1, 2); // prints out:
// -1
// 0
// 1
// 2

logBetween(14, 6); // => prints nothing

logBetween(4, 6); // prints out:
// 4
// 5
// 6
```

### Print Fives

```javascript
function printFives(max) {
    for (let i = 0; i < max; i += 5) {
        console.log(i);
    }
}

// Example:

printFives(20) // prints out:
// 0
// 5
// 10
// 15
```

### Log Between Stepper

```javascript
function logBetweenStepper(min, max, step) {
    for (let i = min; i <= max; i += step) {
        console.log(i);
    }
}

// Examples:
logBetweenStepper(5, 9, 1); // prints out:
// 5
// 6
// 7
// 8
// 9


logBetweenStepper(-10, 15, 5)  // prints out:
// -10
// -5
// 0
// 5
// 10
// 15
```

### Fizz Buzz

```javascript
function fizzBuzz(max) {
    for (let i = 3; i <= max; i++) {
        const fizz = i % 3 === 0;
        const buzz = i % 5 === 0

        if ((fizz || buzz) && !(fizz && buzz)) {
            console.log(i);
        }
    }
}
// Examples:

fizzBuzz(20); // prints out:
// 3
// 5
// 6
// 9
// 10
// 12
// 18
```

### Add Arrays

```javascript
function combineArray(array1, array2) {
  return array1.concat(array2);
}

console.log(combineArray([1, 2], [3, 4])); // => [1, 2, 3, 4]
console.log(combineArray([17, 5], [6, 7]));  // => [17, 5, 6, 7]
```

### Doubler

```javascript
function doubler(numbers) {
    return numbers.map(a => a * 2);
}

console.log(doubler([1, 2, 3, 4])); // => [2, 4, 6, 8]
console.log(doubler([7, 1, 8])); // => [14, 2, 16]
```

### Vowel Counter

```javascript
function countVowels(word) {
  const vowels = "aeiou".split('');
  const isVowel = letter => vowels.includes(letter);
  return word.split('').filter(isVowel).length;
};

console.log(countVowels("bootcamp")); // => 3
console.log(countVowels("apple")); // => 2
console.log(countVowels("pizza")); // => 2
```



## Setting Up Your Environment I

## HTML & CSS Fundamentals

## Intermediate HTML & CSS

## HTML & CSS: Putting It All Together

## Setting Up Your Environment II

## Intermediate JavaScript
