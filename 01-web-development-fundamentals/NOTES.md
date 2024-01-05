# Web Development Fundamentals

## Getting Started at App Academy

### Documenting My Expectations

- each section corresponds to roughly one day of bootcamp
- click through links for additional reading
- learn actively by engaging with the material

### What makes a good question?

- It's specific
- It's clear and concise
- It shows that you've put work into it


### The Secret to Solving any Problem
George Polya


- Understand the problem
- Make a plan
- Carry out the plan
- Look back and improve your solution

## JavaScript Fundamentals

### Data Types

#### Number

All numbers, integers and decimals, positive and negative

##### The basic arithmetic operators

- `+` (addition)
- `-` (subtraction)
- `*` (multiplication)
- `/` (division)
- `%` (modulo)

###### Assignment Shorthand
```javascript
let number = 0;
number += 10; // equivalent to number = number + 10
number -= 2; // equivalent to number = number - 2
number /= 4; // equivalent to number = number / 4
number *= 7; // equivalent to number = number * 7
console.log(number); // 14
```

Any nonsensical arithmetic will result in `NaN`

#### Boolean

##### Logical Operators

We can write boolean expressions that consist of multiple logical operations, but we should be aware of the order of operations. JavaScript will evaluate `!` then `&&` then `||`.

- `!` (not)
- `&&` (and)
- `||` (or)


##### De Morgan's Law
A common mistake in boolean logic is to incorrectly distribute ! across parentheses. Say we had boolean values of A, B. Here is something to remember:

- `!(A || B)` is equivalent to `!A && !B`
- `!(A && B)` is equivalent to `!A || !B`

#### String


- a String is a data type that contains multiple characters enclosed in quotation marks
- `string.length` returns the number of characters in the string
each character of a string is associated with a number index; the first character of a string is at index 0
- `string.indexOf(char)` to obtain the index of char within string; if char is not found, then -1 is returned
- `+` to concatenate multiple strings, combining them into a single string


### Variables

Used to store information to be referenced later

Initialize a variable: `let variableName = "12";`

Declare a variable: `let variableName`, declaring a variable will set the contents of that variable to `undefined` until it is assigned a value

Assign a variable `variableName = "12"` assigns a value to a variable previously declared. Repeat the process to assign a new value to the variable. Variables declared with `const` rather than `let` cannot be re-assigned.

### Functions

A function is a set of code that will run when called.

A function definition consists of the function keyword, followed by three things:

- The name of the function.
- A list of parameters to the function, enclosed in parentheses (`( )`).
- The code to be run when this function is run, enclosed in curly braces (`{ }`).

When we invoke or call a function, we specify the data for a function to use. When we specify what data to use for a function call, we refer to that process as passing arguments to the function.

Every function in JavaScript returns `undefined` unless otherwise specified.


**Parameters** are comma separated variables specified as part of a function's declaration.

**Arguments** are values passed to the function when it is invoked.

### Control Flow

#### Conditionals

`if`, `else if`, `if...else`

```javascript
function mathFun() {
  let x = 19;
  if (x === 3) {
    console.log("we have a 3");
  } else if (x === 4) {
    console.log("we have a 4");
  } else {
    console.log("I will return if everything above me is falsey!");
  }
};

mathFun(); // => "I will return if everything above me is falsey!"
```

#### Loops

##### While Loop

```javascript
let index = 0;

// this is the condition that will be checked every time this loop is run
while (index < 10) {
  console.log("The number is " + index);
  // this is common shorthand for index = index + 1
  index++;
}
```

##### For Loop

```javascript
let testString = "testing";

// We can use the testString's length as our condition!
// Since we know the testString's index starts at 0
// and our index starts at 0 we can access each letter:
for (let index = 0; index < testString.length; index += 1) {
  let letter = testString[index];
  console.log(letter);
}
```

#### Arrays

```javascript
let wackyArray = [2, 17, "apple", "cat", ["apple"]];

console.log(wackyArray[0]); // => 2
console.log(wackyArray[1]); // => 17
console.log(wackyArray[3]); // => "cat"
console.log(wackyArray[4]); // => ["apple"]
```


Get value at a particular index of an array with square brackets `[]`

| method     |                      |
| ---------- | -------------------- |
| .indexOf() | find index of value  |
| .length    | find length of array |
| .concat()  | concatenate          |
| .push()    | add to end           |
| .pop()     | remove from end      |
| .shift()   | add to start         |
| .unshift() | remove from start    |

## Setting Up Your Environment I
My mac was already setup, so I just double checked that I had each of the required programs available on my mac.

- updated python3 version
- updated nodejs version

Note: on a mac with both Python 2 and Python 3 installed, you have to use `pip3 install pipenv` instead of `pip install pipenv`, otherwise you're installing pipenv for version 2 of Python, rather than version 3 (the version this course uses).

### Shell commands

| command |                                               |
| ------- | --------------------------------------------- |
| ls      | list the contents of a directory              |
| clear   | clear the terminal                            |
| echo    | output a string or the contents of a variable |
| pwd     | print current directory                       |
| ls      | list directory contents                       |
| cd      | change directory                              |
| mkdir   | create a new directory                        |
| mv      | move a file or directory                      |
| cp      | copy a file or directory                      |
| rm      | remove a file or directory                    |

### Git commands

| command  |                                     |
| -------- | ----------------------------------- |
| checkout | checkout new branch                 |
| clone    | clone a remote repository           |
| commit   | commit changes to local repository  |
| push     | push changes to remote repository   |
| pull     | pull changes from remote repository |
| status   | print current branch and status     |


## HTML & CSS Fundamentals
When setting up any HTML document, you start by using the four basic parts, which we will call "tags": html, head, title and body.

Attributes are used to define additional information about an element. They are located inside the opening tag, and usually come in name/value pairs (name= “value”).

Each value for the "id" attribute must be unique across the entire HTML document. That gives each element its own unique identifier that you can use as a CSS selector to apply styling to one specific element.

The "class" attribute is another way for CSS to be able to select HTML elements. Classes are meant to be applied to more than one element. That means that there's nothing wrong with the following HTML even though the paragraph tags have the same class value. (Note that the ids are different, though.)

| element      |                                                                                                                                                                                                                                                                                                                                             |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| html         | The HTML html element represents the root (top-level element) of an HTML document, so it is also referred to as the root element. All other elements must be descendants of this element.                                                                                                                                                   |
| head         | The HTML head element contains machine-readable information (metadata) about the document, like its title, scripts, and style sheets.                                                                                                                                                                                                       |
| body         | The HTML body element represents the content of an HTML document. There can be only one body element in a document                                                                                                                                                                                                                          |
| link         | The HTML External Resource Link element (link) specifies relationships between the current document and an external resource. This element is most commonly used to link to stylesheets, but is also used to establish site icons (both "favicon" style icons and icons for the home screen and apps on mobile devices) among other things. |
| title        | The HTML Title element (title) defines the document's title that is shown in a browser's title bar or a page's tab.                                                                                                                                                                                                                         |
| footer       | The HTML footer element represents a footer for its nearest sectioning content or sectioning root element. A footer typically contains information about the author of the section, copyright data or links to related documents.                                                                                                           |
| header       | The HTML header element represents introductory content, typically a group of introductory or navigational aids. It may contain some heading elements but also a logo, a search form, an author name, and other elements.                                                                                                                   |
| h1, h2, etc. | The HTML h1–h6 elements represent six levels of section headings. h1 is the highest section level and h6 is the lowest.                                                                                                                                                                                                                     |
| main         | The HTML main element represents the dominant content of the body of a document. The main content area consists of content that is directly related to or expands upon the central topic of a document, or the central functionality of an application.                                                                                     |
| nav          | The HTML nav element represents a section of a page whose purpose is to provide navigation links, either within the current document or to other documents. Common examples of navigation sections are menus, tables of contents, and indexes.                                                                                              |
| section      | The HTML section element represents a standalone section — which doesn't have a more specific semantic element to represent it — contained within an HTML document.                                                                                                                                                                         |
| div          | The HTML Content Division element (div) is the generic container for flow content. It has no effect on the content or layout until styled using CSS.                                                                                                                                                                                        |
| li           | The HTML li element is used to represent an item in a list.                                                                                                                                                                                                                                                                                 |
| ol           |                                                                                                                                                                                                                                                                                                                                             | The HTML ol element represents an ordered list of items — typically rendered as a numbered list. |
| p            | The HTML p element represents a paragraph.                                                                                                                                                                                                                                                                                                  |
| ul           | The HTML ul element represents an unordered list of items, typically rendered as a bulleted list.                                                                                                                                                                                                                                           |
| a            | The HTML a element (or anchor element), with its href attribute, creates a hyperlink to web pages, files, email addresses, locations in the same page, or anything else a URL can address.                                                                                                                                                  |
| br           | The HTML br element produces a line break in text (carriage-return). It is useful for writing a poem or an address, where the division of lines is significant.                                                                                                                                                                             |
| em           | The HTML em element marks text that has stress emphasis. The em element can be nested, with each level of nesting indicating a greater degree of emphasis.                                                                                                                                                                                  |
| span         | The HTML span element is a generic inline container for phrasing content, which does not inherently represent anything. It can be used to group elements for styling purposes (using the class or id attributes), or because they share attribute values, such as lang.                                                                     |
| strong       | The HTML Strong Importance Element (strong) indicates that its contents have strong importance, seriousness, or urgency. Browsers typically render the contents in bold type.                                                                                                                                                               |
| img          | The HTML img element embeds an image into the document.                                                                                                                                                                                                                                                                                     |

### CSS Basics

#### CSS Selectors

| selector                   |                                                                                                                                                                                  |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Type selectors             | matches elements by node name (e.g. div, li, a, p)                                                                                                                               |
| Class selectors            | matches elements by class name (e.g. `<button class=“active”>)`                                                                                                                  |
| ID selectors               | matches elements by ID name (e.g. `<div id=”list-1”>`)                                                                                                                           |
| Universal selectors        | matches elements of any type (e.g. `*`)                                                                                                                                          |
| Attribute selectors        | matches elements based on the presence or value of a given attribute (e.g. a[title] matches all a elements with a title attribute)                                               |
| Descendant selectors       | `p abbr{}`                    matches element `abbr` that is a decendent of `p`                                                                                                  |
| Compound class selectors   | combination of two classes (with no space) like `.box.orange `                                                                                                                   |
| Direct child selector      | The > selector selects nodes that are direct children of the first element  (`.menu > .is-active`)                                                                               |
| Adjacent sibling selectors | The + selector selects adjacent siblings    (syntax: A + B). This means that the second element (B) directly follows the first (A), and both share the same parent. `h1 + h2 {}` |
| Pseudo-selectors           | ::before, ::after                                                                                                                                                                |
| Pseudo-classes             |
- active: applies to elements like buttons when activated by a person, like when they "push down" on the button
- checked: applies to radio inputs, checkbox inputs, and options in drop downs when the user has toggled it into an "on" state
- disabled: applies to any disabled element, like a disabled button or input
- first-child: applies to the first element among a group of sibling elements
- focus: applies to elements that have the current focus, like inputs and buttons
- hover: applies to elements that currently have the pointing device (cursor) directly over it (it is problematic on touchscreens because it may never match the element because there is no persistent pointing device)
- invalid: applies to any form element in an invalid state due to client-side form validation
- last-child: applies to the last element among a group of sibling elements
- not(selector): represents elements that do not match the provided selector
- required: applies to form elements that are required
- valid: applies to any form element in a valid state
- visited: applies to anchor tags of which the user has already been to the URL that the href points to



## Intermediate HTML & CSS

### HTML Forms
```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="utf-8">
    <title>Learning the Forms</title>
  </head>
  <body>
    <h1>Hello, Forms!</h1>
    <form action="/form-handling-url" method="post">
      <fieldset>
        <legend>Add user</legend>

        <div>
          <label for="firstName">First name</label>
          <input type="text" id="firstName" name="first_name">
        </div>

        <div>
          <label for="lastName">Last name</label>
          <input type="text" id="lastName" name="last_name">
        </div>

        <div>
          <label for="email">Email</label>
          <input type="email" id="email" name="email_address">
        </div>

        <div>
          <label for="role">Role</label>
          <select id="role" name="user_role_name">
            <option value="admin">Admin</option>
            <option value="user">User</option>
            <option value="guest">Guest</option>
          </select>
        </div>

        <div>
          <label for="expiration">Expiration</label>
          <input type="date" id="expiration" name="expiration">
        </div>

        <div>
          <label for="bio">Bio</label>
          <textarea id="bio" name="bio"></textarea>
        </div>

        <div>
          <button type="submit">Add this person</button>
        </div>

      </fieldset>
    </form>

  </body>
</html>
```

### HTML Elements II

#### Tables
| Element |                                                                                                                                                                    |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| table   | The HTML table element represents tabular data — that is, information presented in a two-dimensional table comprised of rows and columns of cells containing data. |
| tbody   | The HTML Table Body element (tbody) encapsulates a set of table rows (tr elements), indicating that they comprise the body of the table (table).                   |
| td      | The HTML td element defines a cell of a table that contains data. It participates in the table model.                                                              |
| tfoot   | The HTML tfoot element defines a set of rows summarizing the columns of the table.                                                                                 |
| th      | The HTML th element defines a cell as header of a group of table cells. The exact nature of this group is defined by the scope and headers attributes.             |
| thead   | The HTML thead element defines a set of rows defining the head of the columns of the table.                                                                        |
| tr      | The HTML tr element defines a row of cells in a table. The row's cells can then be established using a mix of td (data cell) and th (header cell) elements.        |

#### Forms

| Element  |                                                                                                                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| button   | The HTML button element represents a clickable button, which can be used in forms or anywhere in a document that needs simple, standard button functionality.                                                                             |
| fieldset | The HTML fieldset element is used to group several controls as well as labels (label) within a web form.                                                                                                                                  |
| form     | The HTML form element represents a document section that contains interactive controls for submitting information to a web server.                                                                                                        |
| input    | The HTML input element is used to create interactive controls for web-based forms in order to accept data from the user; a wide variety of types of input data and control widgets are available, depending on the device and user agent. |
| label    | The HTML label element represents a caption for an item in a user interface.                                                                                                                                                              |
| legend   | The HTML legend element represents a caption for the content of its parent fieldset.                                                                                                                                                      |
| option   | The HTML option element is used to define an item contained in a select, an optgroup, or a datalist element. As such, option can represent menu items in popups and other lists of items in an HTML document.                             |
| select   | The HTML select element represents a control that provides a menu of options                                                                                                                                                              |
| textarea | The HTML textarea element represents a multi-line plain-text editing control, useful when you want to allow users to enter a sizable amount of free-form text, for example a comment on a review or feedback form.                        |

### Intermediate CSS

In the standard Box Model, the width and height of an element set with CSS refers to the width and height of the box's content. Any padding, border and margin added to the element will get added to the total size of actual box. If padding, border or margin are removed from a box, the box size decreases, but the width and height of the content stays the same.

The CSS position property accepts any of the following five values:

- Static
- Relative
- Absolute
- Fixed (like absolute, but relative to the page, not parent)
- Sticky

#### CSS Transitions
| Property            |                                                                                                                                                                                                                                              |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| transition-property | Specifies the name or names of the CSS properties to which transitions should be applied. Only properties listed here are animated during transitions; changes to all other properties occur instantaneously as usual.                       |
| transition-duration | Specifies the duration over which transitions should occur. You can specify a single duration that applies to all properties during the transition, or multiple values to allow each property to transition over a different period of time. |
| transition-delay    | Defines how long to wait between the time a property is changed and the transition actually begins.                                                                                                                                          |

#### CSS Animation
```css
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}

div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}
```
## HTML & CSS: Putting It All Together

## Setting Up Your Environment II

## Intermediate JavaScript
