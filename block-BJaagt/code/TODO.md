Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // username is not defined
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // username is not defined
```
In the above code we are looking for the variable name `username`. There is no variable named `username` in the global scope. The variable is inside the curly braces and it can't be accesed from outside.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // username is not defined
```
In the above code we are looking for the variable name `username`. There is no variable named `username` in the global scope. The variable is inside the block scope and it can't be accesed from outside.

The above code will throw an error `Reference Error username is not defined`.


4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // Arya
```
In the above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable inside the block scope can't be accesed from outside.

The above code  Output will be Arya.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); //  'username' has already been declared.
```
In the above code we are looking for the variable named `username` but inside the if statement again var is created using same variable name so it will throw an error.

The error will be username is allready been declared.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // 'john'
```

In the above code we are looking for the variable named `username`. In the global scope username is 'john'.

Output will be 'john'.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // 'john'
```
In the above code we are looking for the variable named `username`. In the global scope username is 'john'.

Output will be 'john'.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 1 2 3 4 5 6 7 8 9
}
console.log(i, 'Second'); // 10
```
In the above code `i` is created using var and var is not block scoped so we can access the value of `i` globaly.

Output will be 0 'First'
               1 'First'
               2 'First'
               3 'First'
               4 'First'
               5 'First'
               6 'First'
               7 'First'
               8 'First'
               9 'First'
              10 'Second'

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 1 2 3 4 5 6 7 8 9 
}
console.log(i, 'Second'); // i is not defined
```
In the above scope `i` is created using let and let is block as well as function scope so from outside the loop it will not be accesed.
 
Output will be 0 1 2 3 4 5 6 7 8 9.