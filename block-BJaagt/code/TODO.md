Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block scope and we have used const to declare it.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block scope and we have used let to declare it.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output 'Arya'
```
In above code we are looking for the variable named `username`. There is a variable named `username` in the global scope.The variable is inside the block scope and we have used var to declare it. So it would be available in the global scope too.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output
```
At the start the username would be empty. Then it would be initialized with undefined. After that it would be given a value of 'John' but then it would be given a value of 'Arya', but then it would show syntax error, the value has already been declared

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output 'John'
```
Since Arya is declared using let and since it's block scoped, and username is declared as John in the global scope. We get the output as John

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output 'John'
```
Since Arya is declared using let and since it's function scoped, and username is declared as John in the global scope. We get the output as John

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output 0 'First'
}
console.log(i, 'Second'); // output 10 'Second'
```
It starts in the loop from 0 to 10. But when it comes out of the loop the value of i would be 10.

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
It starts in the loop from 0 to 10. But since i is declared using let and since its block scoped, the second part would give a reference error since i would not be defined.