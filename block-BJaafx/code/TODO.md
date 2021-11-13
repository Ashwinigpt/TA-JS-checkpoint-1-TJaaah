1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
 let sum = 0;
  for(let a = 1; a <= 10; a++) {
    let num = +prompt("Enter number")
    sum = sum + a;
    average = sum / 10;
  }
  console.log(average);
} 
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
The output of the code will be error because in this code 'println' is not defined.

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum(max) {
  let sum = 0;
  for(let a = 0; a <= 10; a = a + 2) {
    sum = sum + a;
  }
  console.log(sum);
} 
getEvenSum(10);
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max) {
  let sum = 0;
  for(let a = 1; a < 10; a = a + 2) {
    sum = sum + a;
  }
  console.log(sum);
} 
getOddSum(10);
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js
function getProductOfDigits(num) {
  if (num < 0) {
    return `not a valid input`
  }
let product = 1;
for(let a = 0; a < num.length; a++) {
  product = product * (num[a]);
}
console.log(product);
}
```

```js
function getProductOfDigits(num) {
  if (num < 0) {
    return `not a valid input`
  }
  let product = 1
  while(num > 0) {
    let reminder = num % 10
    num = num - reminder
    product = product * reminder
    num = num/10
  }
return product
}

```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); 'Bigger than 5' because 10 is greater than 5 and we put in condition-1 that if num > 5, it returns 'Bigger than 5'.
check(1); 'Smaller than 5' because 1 is lower than 5 and we put in condition-2 that if num < 5, it returns `Smaller than 5'
check(5); 'num' because we have put in condition if above both condition is not matching then it returns `num`.  
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); 'You are arya' because we put `Arya` in name and condition is if name = `Arya` then it returns 'You are arya'
getOutput('John'); 'You are john' because we put `John` in name and condition is if name = `John` then it returns 'You are John'
getOutput(); 'Who are you' because we have put in condition if above both condition is not matching then it returns `Who are you`
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); 'You are arya' 'Who are you' because we put console.log and return both so output will be both.
getOutput('John'); 'You are john' 'Who are you' because we put console.log and return both so output will be both.
getOutput(); 'Who are you' because both above condition is not matching so returns the last one.
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

Yes, a function can have multiple return statement.
```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}
getOutput('Arya'); 'You are arya' because we put `Arya` in name and condition is if name = `Arya` then it returns 'You are arya'
getOutput('John'); 'You are john' because we put `John` in name and condition is if name = `John` then it returns 'You are John'
getOutput(); 'Who are you' because we have put in condition if above both condition is not matching then it returns `Who are you`

```

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

The difference between for loop and while loop is that in for loop the number of iterations to be done is already known and is used to obtain a certain result whereas in while loop the command runs until a certain condition is reached and the statement is proved to be false.

In general, we should use a for loop when we know how many times the loop should run. If we want the loop to break based on a condition other than the number of times it runs, we should use a while loop.

```js

for (let a = 0; a <= 5; a++) {
  console.log(i);
}

```
```js

let a = 0;
while (a < 10) {
  a++;
  console.log(a);
  }

```