1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
function sum(a, b) {
  return a + b;
} it returns a + b

function sum(a, b) {
  console.log(a + b);
}  it console a + b and returns undefined.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

The value of first = a + b, and the value of second = undefined.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

function sum(a, b) {
  return a + b;
}
sum(12, 24, 35);

The output will be 36 because third parameter has not defined so 35 will not be added.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

Yes, we can store the first `sum` function in a variable named `add` because function is a expression and expression could be stored in any variable.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

function sayHello (name) {
  return (`Hello ${name}`);
}
sayHello("Arya");

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
The output of the function below is 'Hello, John'. because we put `John` in username.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); John

showMessage(); 'Hello, John'

alert(userName); John
```

8. What is a Anonymous Function give example of three functions.

An anonymous function is a function without a name.

let addNum = function (numA, numB) {
  return numA + numB;
}
addNum(10, 21);


let sum = function (firstName, lastName) {
  return `${firstName} ${lastName}`
}
sum("Ashwini","Gupta");


let square = function (num1) {
  return num1**2;
}
square(5);

9. Can function declaration be a Anonymous Function? Explain

No, function declaration can not be a Anonymous Function because in anonymous function we have to put a variable but in function declaration it not be needed.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

function getFullName(firstName , lastName) {
  return `${firstName} ${lastName}`;
}
getFullName("John", "Snow"); 


let calcSquare = function (num1) {
  return num1**2;
}
calcSquare(5);


function createSum(a, b) {
  return a + b;
}
createSum(2, 4);


function checkBoolean () {
  let year = prompt("Enter a year");
  if(year % 4 === 0 && year % 400 === 0) {
    alert (true);
  } else {
    alert(false);
  }
}

checkBoolean();

