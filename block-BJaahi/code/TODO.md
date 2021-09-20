For the given code below:

- re-write the code in ways that system will understand

For Example:

1.

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
```

2.

```js
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```
```js
<!-- Answer -->
// Declaration phase
var username = undefined;
let number;
function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution phase
Uncaught ReferenceError: numbers is not defined
```

3.

```js
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase
var username = undefined;
let number;
let sayHello = fn();

let message;
var nextMessage = undefined;


//Execution phase
Uncaught ReferenceError: numbers is not defined
```

4.

```js
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
//Declaration phase
let username;
let number;
let message;
let sayHello;
var nextMessage=undefined;
//Execution phase
let username ='Arya';
Uncaught ReferenceError: numbers is not defined
```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->

```js
// declaration phase
var name=undefined;
let age;

// execution phase
Error:  age not defined
```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->

```js
//declaration phase


//execution phase
sayhi();
//declaration phase
var name =undefined;
let age ;
//execution phase
Error :age not defined
```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->

```js
//declaration phase


//execution phase
sayhi();
//declaration phase
var name =undefined;
let age ;
//execution phase
Error :age not access before initialisation

```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->

```js
//declaration phase
let sayHi ;

//execution phase
let sayHi =fn();
function sayHi(){
  console.log(name);
  console.log(age);
  //declaration phase
  var name = undefined;
  let age ;

  //execution phase 
  Error :age cannot be accessed before initialisation
}
```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->

```js
// declaration phase
let num1;
var sum=undefined;
let num2;

//execution phase
let num =21;
Error : num2 is not defined;
```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->

```js
//declaration phase
var num1 =undefined;
let sum2 ;
let add;
let num2;
let sum;

//execution phase
let num=21;
let sum =fn;
error : addAgain not defined
```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->

```js
// declaration phase
let sum;
let add;
//execution phase
let sum = test(100);
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
// declaration phase
let sum;
// execution phase
let sum= fn;
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
function add(a, b) {
  return a + b;
}

```
