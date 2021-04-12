1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
```
let percentage = (marks,total) => {
  return (marks * 100) / total;
}

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
```Function Declaration

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```Function Expression

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```Function Expression

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```Function Expression

```js
let percentage = (marks, total) => (marks * 100) / total;
```Function Expression

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
Because the function keyword can be used to define a function in an expression
const area = function(length, height){
  return width*height
}
4. Why is a function call an expression in JavaScript?

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer VALID
five = add; // Answer VALID
five = five(10, 11); // Answer VALID
five = function () {
  return 'Hello';
}; // Answer VALID
```

6. What is the difference between function definition and function call? Explain with an example.
let percentage = (marks, total) => (marks * 100) / total; 
is a function definition and 
percentage(67,100) is a function call

7. What is the similarities between function definition and function call?


8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid
```valid

9. What is higher order function explain with an example.
Higher-order functions are functions that take other functions as arguments or return functions as their results.
const double = n => n * 2
[1, 2, 3, 4].map(double)

10. Explain what is callback function. Why you can pass a function inside a function?
A callback is a function passed into another function as an argument to be executed later.
