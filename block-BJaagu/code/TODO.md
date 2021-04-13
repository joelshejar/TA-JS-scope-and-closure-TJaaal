Find the output of the code snippets below:

```js
console.log(numA + numB); //OUTPUT
var numA = 21,
  numB = 30;
```NaN

Find the output of the code snippets below:

```js
console.log(numA + numB); //OUTPUT
let numA = 21,
  numB = 30;
```ReferenceError

Find the output of the code snippets below:

```js
let numA = 21,
  numB = 30;
console.log(numA + numB); //OUTPUT
```51

Find the output of the code snippets below:

```js
console.log(sayHello()); // OUTPUT
function sayHello() {
  console.log("Hey");
}
function sayHello() {
  console.log("Hello");
}
```Hello

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // OUTPUT 
function sayHello() {
  console.log(username);
}
``` Tyrion

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT
let username = "Tyrion";
function sayHello() {
  console.log(username);
}
```ReferenceError

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // OUTPUT
let sayHello = () => {
  console.log(username);
};
```ReferenceError

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT
let username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```ReferenceError

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```ReferenceError

Find the output of the code snippets below:

```js
var username = "Tyrion";
sayHello(); // OUTPUT
let sayHello = () => {
  console.log(username);
};
```ReferenceError

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  var username = "John";
};
sayHello(); // OUTPUT
```undefined

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  var username = "John";
  console.log(username);
};
sayHello(); // OUTPUT
```John

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  let username = "John";
};
sayHello(); // OUTPUT
```ReferenceError
