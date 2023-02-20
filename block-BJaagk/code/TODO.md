1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function (marks, total) {
  return (marks * 100) / total;
}

let percentage = (marks, total) => {
  return (marks * 100) / total;
}

let percentage = (marks, total) => (marks * 100) / total;
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
function declaration

```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total; // function expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
// When we assign any function to any variable while declaring it then it is called function expression.
    
    function percentage(marks, total) {
  return (marks * 100) / total;
};

4. Why is a function call an expression in JavaScript?
// A function is taken as an expression in javaScript and function in JavaScript is an object and it can be 
   assign it to any variable.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer   valid 5;
five = add; // Answer             valid;   
five = five(10, 11); // Answer    valid 21; 
five = function () {
  return 'Hello';
}; // Answer                      valid;
```

6. What is the difference between function definition and function call? Explain with an example.
// Whenever we define a functions with a certain steps is called function definition and when we call it with 
   paranthesis is called function call.
```js 
// function definition 
   function add(a, b) {
    return a + b;
   }

// fuction call
   add(5, 4);   
```
7. What is the similarities between function definition and function call?
// function defination is an expression (functions is an object) 
// function call is an expression (function call always returns a value)

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid because hello is a function and it can store key and value.
```

9. What is higher order function explain with an example.
// function which accepts functon as an arguments is called higher order function.
// it accepts a function function definition and returns a function definiton.

10. Explain what is callback function. Why you can pass a function inside a function?
// A function passed as an argument in another function is called callback function.