# JavaScript Fundamentals

## Hello World

```javascript
// Here is an example of using console.log to print a message:

console.log('hello world');

// Print out your own message using console.log below:
console.log("Hello"); // Hello
```

## Favorite Food

```javascript
// Here is an example of using console.log:

console.log('cereal');

// Print out your favorite food using console.log below:
console.log("Red beans and rice");
```

## Numbers Exercise

```javascript
// Example:
console.log(4 + 2.5)   // 6.5

// Write 5 more expressions below:
console.log(4 + 2.5)  // 6.5
console.log(100 - 20) // 80
console.log(4 * 0.5)  // 2
console.log(20 / 5)   // 4
console.log(13 % 3)   // 1
```

## Strings Exercise

```javascript
// Example:
console.log('hello ' + 'world');  // 'hello world'

// Write 3 more expressions below:
console.log('hello ' + 'world');  // 'hello world'
console.log('down' + 'the' + 'rabbithole');   // 'downtherabbithole'
console.log('abcdef'[4]);   // 'e'
console.log('whoa'.length);   // 4
```

## addLib Problem

```javascript
function makeAddLib(verb, adj, noun) {
  return `I shall ${verb} to the ${adj} ${noun}`;
}


console.log(makeAddLib("swim", "sparkly", "rainbow")); // => "I shall swim to the sparkly rainbow?"
console.log(makeAddLib("RUN", "FANCY", "ParK")); // => "I shall RUN to the FANCY ParK?"
```

## Goodbye

```javascript
function goodbye(name) {
  return `Bye ${name}.`
}

console.log(goodbye("Daniel")); // => "Bye Daniel."
console.log(goodbye("Mark")); // => "Bye Mark."
console.log(goodbye("Beyonce")); // => "Bye Beyonce."
```

## Plus Five

```javascript
function plusFive(num) {
  return num + 5;
}

console.log(plusFive(10));  // => 15
console.log(plusFive(2));   // => 7
console.log(plusFive(-8));  // => -3
```

## Call This Function

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

## Average of Two

```javascript
function averageOfTwo(num1, num2) {
  return (num1 + num2) / 2;
}

console.log(averageOfTwo(3, 7)); // => 5
console.log(averageOfTwo(16, 5)); // => 10.5
console.log(averageOfTwo(2, 7.5)); // => 4.75
```

## Hello

```javascript
function hello(str) {
  console.log(`Hello, ${str}`);
}

hello("cat"); // prints "Hello, cat"
hello("Helen"); // prints "Hello, Helen"
hello("Sting"); // prints "Hello, Sting"
```

## Divide by Three

```javascript
function divideByThree(num) {
  return num / 3;
}

console.log(divideByThree(9)); // => 3
console.log(divideByThree(15)); // => 5
console.log(divideByThree(98)); // => 32.666666666666664
```

## Whisper

```javascript
function whisper(str) {
  return `...${str.toLowerCase()}...`
}

console.log(whisper("Hey Buddy")); // => "...hey buddy..."
console.log(whisper("YEA! that was fun")); // => "...yea! that was fun..."
```

## Average of Four

```javascript
function averageOfFour(num1, num2, num3, num4) {
    return (num1 + num2 + num3 + num4) / 4;
}

console.log(averageOfFour(10, 10, 15, 5)); // => 10
console.log(averageOfFour(3, 10, 11, 4)); // => 7
console.log(averageOfFour(1, 2, 3, 4)); // => 2.5
```

## Yell

```javascript
function yell(str) {
  return `${str.toUpperCase()}!!!`;
}

console.log(yell("I want to go to the store")); // => "I WANT TO GO TO THE STORE!!!"
console.log(yell("Time to program")); // => "TIME TO PROGRAM!!!"
```

## Echo

```javascript
function echo(string) {
    console.log(`${string.toUpperCase()} ... ${string} ... ${string.toLowerCase()}`);
}

echo("Mom!"); // => prints "MOM! ... Mom! ... mom!"
echo("hey"); // => prints "HEY ... hey ... hey"
echo("JUMp"); // => prints "JUMP ... JUMp ... jump"
```

## Is Five

```javascript
function isFive(num) {
  return num === 5;
}

console.log(isFive(5)); // => true
console.log(isFive(13)); // => false
```

## Is Odd

```javascript
function isOdd(num) {
  return num % 2 !== 0;
}

console.log(isOdd(2)); // => false
console.log(isOdd(5)); // => true
console.log(isOdd(-17)); // => true
```

## Is Substring

```javascript
function isSubstring(searchString, subString) {
  return searchString.toLowerCase().indexOf(subString.toLowerCase()) !== -1;
}

console.log(isSubstring("The cat went to the store", "he cat went")); // => true
console.log(isSubstring("Time to program", "time")); // => true
console.log(isSubstring("Jump for joy", "joys")); // => false
```

## Three or Seven

```javascript
function threeOrSeven(num) {
  return num % 3 === 0 || num % 7 === 0;
}

console.log(threeOrSeven(3));   // => true
console.log(threeOrSeven(42));  // => true
console.log(threeOrSeven(8));   // => false
```

## String Included

```javascript
function eitherStringIncluded(sentence, word1, word2) {
    return sentence.includes(word1) || sentence.includes(word2);
}

console.log(eitherStringIncluded("how now brown cow?", "panther", "cow")); //=> true
console.log(eitherStringIncluded("Question?", "Answer", "?")); //=> true
console.log(eitherStringIncluded("I love programming", "apple", "potato")); //=> false
console.log(eitherStringIncluded("Dance party!", "?", "what")); //=> false
```

## Log Between

```javascript
function logBetween(lowNum, highNum) {
    for (let i = lowNum; i <= highNum; i++) {
        console.log(i);
    }
}
// Examples:
logBetween(-1, 2); // prints out:
-1
0
1
2

logBetween(14, 6); // => prints nothing

logBetween(4, 6); // prints out:
4
5
6
```

## Print Fives

```javascript
function printFives(max) {
    for (let i = 0; i < max; i += 5) {
        console.log(i);
    }
}
// Example:

printFives(20) // prints out:
0
5
10
15
```

## Log Between Stepper

```javascript
function logBetweenStepper(min, max, step) {
    for (let i = min; i <= max; i += step) {
        console.log(i);
    }
}

// Examples:
logBetweenStepper(5, 9, 1); // prints out:
5
6
7
8
9


logBetweenStepper(-10, 15, 5)  // prints out:
-10
-5
0
5
10
15
```

## Fizz Buzz

```javascript
function fizzBuzz(max) {
    for (let i = 3; i < max; i++) {
        const byThree = i % 3 === 0;
        const byFive = i % 5 === 0;
        if ((byThree || byFive) && !(byThree && byFive)) {
            console.log(i);
        }
    }
}
// Examples:

fizzBuzz(20); // prints out:
3
5
6
9
10
12
18
```

## Dynamic Fizz Buzz

```javascript
function dynamicFizzBuzz(max, num1, num2) {
    const result = [];
    for (let i = 0; i < max; i++) {
        const byFirst = i % num1 === 0;
        const bySecond = i % num2 === 0;
        if ((byFirst || bySecond) && !(byFirst && bySecond)) {
            result.push(i);
        }
    }
    return result;
}



console.log(dynamicFizzBuzz(20, 3, 5)); // [ 3, 5, 6, 9, 10, 12, 18 ]
console.log(dynamicFizzBuzz(24, 4, 6)); // [ 4, 6, 8, 16, 18, 20 ]
```

## Least Common Multiple

```javascript
function  leastCommonMultiple(num1, num2) {
  const max = num1 * num2;

  // count by increments of num1 up to
  // num1 * num2 which is the multiple
  // of both numbers and, as such, the
  // maximum value the lcm could be
  for (let i = num1; i <= max; i += num1) {
    if (i % num2 === 0) return i;
  }
}

console.log(leastCommonMultiple(4, 6)); // 12
console.log(leastCommonMultiple(3, 5)); // 15
console.log(leastCommonMultiple(2, 10)); // 10
```

## Is Prime

```javascript
function isPrime(num) {
  for (i = 2; i <= num; i++) {
    if (i !== num && num % i === 0) {
      return false;
    }
  }

  return true;
}

console.log(isPrime(2)); // => true
console.log(isPrime(10)); // => false
console.log(isPrime(11)); // => true
console.log(isPrime(9)); // => false
console.log(isPrime(2017)); // => true
```

## Is Perfect Square

```javascript
function isPerfectSquare(num) {
  const root = Math.sqrt(num);
  return num === root * root;
}

console.log(isPerfectSquare(1))     // true
console.log(isPerfectSquare(4))     // true
console.log(isPerfectSquare(64))    // true
console.log(isPerfectSquare(100))   // true
console.log(isPerfectSquare(169))   // true
console.log(isPerfectSquare(2))     // false
console.log(isPerfectSquare(40))    // false
console.log(isPerfectSquare(32))    // false
console.log(isPerfectSquare(50))    // false
```

## Fibonacci

```javascript
function fibonacci(length) {
    // your code here
    if (length === 0) return [];
    if (length === 1) return [1];
    if (length > 1) {
        const result = [1, 1];
        length -= 2;
        while (length > 0) {
            result.push(result[result.length - 1] + result[result.length - 2]);
            length--;
        }
        return result;
    }
}

console.log(fibonacci(0)); // []
console.log(fibonacci(1)); // [1]
console.log(fibonacci(6)); // [1, 1, 2, 3, 5, 8]
console.log(fibonacci(8)); // [1, 1, 2, 3, 5, 8, 13, 21]
```

## While Loop Translation

```javascript
function eCounter(word) {
  let count = 0;
  let index = 0;
  while (index < word.length) {
    index++;
    let char = word[index];
    if (char === "e" || char === "E") {
      count += 1;
    }
  }

  return count;
};

console.log(eCounter("apple")); // => 1
console.log(eCounter("appleapple")); // => 2
console.log(eCounter("Appleee")); // => 3
```

## For Loop Translation

```javascript
function aCounter(word) {
  let count = 0;
  for (let index = 0;index < word.length; index++) {
    let char = word[index];
    if (char === "a" || char === "A") {
      count += 1;
    }

  }
  return count;
};

console.log(aCounter("apple")); // => 1
console.log(aCounter("appleapple")); // => 2
console.log(aCounter("aAapple")); // => 3
```

## Has Vowel

```javascript
function hasVowel(str) {
  return str.match(/[aeiou]/i) !== null;
}

console.log(hasVowel('dog')); // true
console.log(hasVowel('conventional')); // true
console.log(hasVowel('rhythm')); // false
```

## Vowel Counter

```javascript
function countVowels(word) {
  return word.match(/[aeiou]/gi).length;
}

console.log(countVowels("bootcamp")); // => 3
console.log(countVowels("apple")); // => 2
console.log(countVowels("pizza")); // => 2
```

## Pig Latin Slice Research

```javascript
// So the two rules for our version of Pig Latin are:

// 1. For words that start with a vowel, add 'yay' to the end of the word.
// 2. For words that start with a non-vowel, move all letters that come
// **before the first vowel** to the **end of the word** then add 'ay'

function pigLatinWord(word) {
  const firstVowel = word.match(/[aeiou]/i)["index"];
  const start = word.slice(firstVowel);
  const finish = firstVowel === 0 ? "y" : word.slice(0, firstVowel);

  return start + finish + "ay";
}

console.log(pigLatinWord("apple")); //=> "appleyay"
console.log(pigLatinWord("eat")); //=> "eatyay"
console.log(pigLatinWord("banana")); //=> "ananabay"
console.log(pigLatinWord("trash")); //=> "ashtray"
```

## Abbreviate

```javascript
function abbreviate(word) {
  return word.match(/[^aeiou]/gi).join("");
}

console.log(abbreviate('wonderful')); // 'wndrfl'
console.log(abbreviate('mystery')); // 'mystry'
console.log(abbreviate('Accordian')); // 'ccrdn'
```

## Uncompress

```javascript
function uncompress(str) {
  const result = [];
  for (let i = 0; i < str.length; i += 2) {
    const char = str[i];
    const count = +str[i + 1];
    for (j = 1; j <= count; j++) {
      result.push(char);
    }
  }
  return result.join("");
}

console.log(uncompress('x3y4z2')); // 'xxxyyyyzz'
console.log(uncompress('a5b2c4z1')); // 'aaaaabbccccz'
console.log(uncompress('b1o2t1')); // 'boot'
```

## Triplet True

```javascript
function tripletTrue(word) {
  return word.match(/([a-z])\1\1/gi) !== null;
}

console.log(tripletTrue('caaabb'));        // true
console.log(tripletTrue('terrrrrible'));   // true
console.log(tripletTrue('runninggg'));     // true
console.log(tripletTrue('bootcamp'));      // false
console.log(tripletTrue('e'));             // false
```

## Silly Strings

```javascript
function convertVowels(char) {
  return /[aeiou]/.test(char) ? `${char}b${char}` : char;
}
function sillyString(str) {
  return str
    .split("")
    .map((a) => convertVowels(a))
    .join("");
}

console.log(sillyString('stop'));       // stobop
console.log(sillyString('that'));       // thabat
console.log(sillyString('can'));        // caban
console.log(sillyString('cats'));       // cabats
console.log(sillyString('italy'));      // ibitabaly
console.log(sillyString('scooter'));    // scobooboteber
```

## More Dot Less Dash

```javascript
function count(str, char) {
  return str.split("").filter((c) => c === char).length;
}
function moreDotLessDash(str) {
  return count(str, ".") > count(str, "-");
}

console.log(moreDotLessDash('2-D arrays are fun. I think.'));           // true
console.log(moreDotLessDash('Morse code is great.'));                   // true
console.log(moreDotLessDash('.... . -.--'));                            // true
console.log(moreDotLessDash('.--. .-. --- --. .-. .- -- -- . .-.'));    // false
console.log(moreDotLessDash('high-flying acrobat.'));                   // false
```

## Has Three Vowels

```javascript
  const vowelsFound = {};

  for (let i = 0; i < str.length; i++) {
    if (/[aeiou]/.test(str[i])) {
      vowelsFound[str[i]] = true;
    }
  }

  return Object.keys(vowelsFound).length >= 3;
```

## Last Index

```javascript
function lastIndex(str, char) {
  for (let i = str.length - 1; i >= 0; i--) {
    if (str[i] === char) return i;
  }
  return -1;
}

console.log(lastIndex("abca", "a"))        // 3
console.log(lastIndex("mississipi", "i"))  // 9
console.log(lastIndex("octagon", "o"))     // 5
console.log(lastIndex("programming", "m")) // 7
```

## Double Letter Count

```javascript
function doubleLetterCount(string) {
  const doubles = string.match(/([a-z])\1/gi);
  return doubles ? doubles.length : null;
}

console.log(doubleLetterCount("the jeep rolled down the hill"));  // 3
console.log(doubleLetterCount("bootcamp")); // 1
```

## Caesar Cipher

```javascript
function caesar(char, num) {
  // this warrants a special comment
  // since there are 26 letters in the alphabet
  // you can use index % 26 to wrap around
  // past "z" - think about it, z is the 26th letter
  // so the index of "z" (25 because zero based index)
  // plus, say, 1 would be 26 - and 26 % 26 is zero
  // which is the index of a :D
  const alphabet = "abcdefghijklmnopqrstuvwxyz";
  const newIdx = (alphabet.indexOf(char) + num) % 26;
  return alphabet[newIdx];
};

function caesarCipher(string, num) {
  return string
    .split("")
    .map((char) => caesar(char, num))
    .join("");
}
console.log(caesarCipher("apple", 1)); // "bqqmf"
console.log(caesarCipher("bootcamp", 2)); // "dqqvecor"
console.log(caesarCipher("zebra", 4)); // "difve"
```

## Vowel Cipher

```javascript
const vowels = "aeiou";

function shiftVowel(vowel) {
  const newIdx = (vowels.indexOf(vowel) + 1) % 5;
  return vowels[newIdx];
};

function isVowel(vowel) {
  return vowels.indexOf(vowel) >= 0;
}

function vowelCipher(string) {
  return string
    .split("")
    .map((char) => (isVowel(char) ? shiftVowel(char) : char))
    .join("");
}

console.log(vowelCipher("bootcamp")); // "buutcemp"
console.log(vowelCipher("paper cup")); // "pepir cap"
```


## Longest Name - Debugging

```javascript
function longestName(names) {
  // Set the first name to be the longest
  let currentLongest = names[0];

  // Check each other name in the array starting from the second
  for (let i = 1; i < names.length; i++) {
    // If the name we're checking is longer than our
    // current longest, set that name to be the new longest
    if (names[i].length > currentLongest.length) {
      currentLongest = names[i];
    }
  }

  return currentLongest;
}

testNames = ["James", "Patricia", "Michael", "Elizabeth", "Christopher",
             "Sarah", "Margaret", "Kenneth", "Stephanie", "Jonathan",
             "Jeremy", "Samantha", "Alexander", "Catherine", "Benjamin"]

console.log(longestName(testNames)); // "Christopher"
```
