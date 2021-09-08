1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function(marks,total){
                   return (marks * 100)/total;
                 }
let percentage = (marks , total)=>{ return (marks * 100) / total;}

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer 
It is a function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
This is a function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
Function expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
Function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
Function expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

In javascript a function is a object thats why we can assign it to a variable.
ex:: let percentage = (marks, total) => {
  return (marks * 100) / total;
};


4. Why is a function call an expression in JavaScript?
Function Expression  allows us to create an anonymous function which doesn’t have any function name which is the main difference between Function Expression and Function Declaration.A function expression has to be stored in a variable and can be accessed using variableName.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer valid
five = add; // Answer invalid
five = five(10, 11); // Answer invalid
five = function () {
  return 'Hello';
}; // Answer valid
```

6. What is the difference between function definition and function call? Explain with an example.
A function definition provides the actual body of the function.A function definition in C programming consists of a function header and a function body. 
To use a function, you will have to call that function to perform the defined task.
When a program calls a function, the program control is transferred to the called function.
/* calling a function to get max value */
   int ret = max(a, b);
/* function definition */
int max(int num1, int num2) {
  return num1+num2;
}

7. What is the similarities between function definition and function call?
they have the same set of argumnents .

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid   valid
```

9. What is higher order function explain with an example.
A function that accepts other functions as arguments is called a higher-order function, which contains the logic for when the callback function gets executed. 

10. Explain what is callback function. Why you can pass a function inside a function?
A callback function is a function that is passed as an argument to another function, to be “called back” at a later time. 
