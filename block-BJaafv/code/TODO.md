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
console.log is used to print variables and string and dosent break usual flow of functions whereas return is used to return value from a function and stops function execution
2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
30 and undefined
3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
  NaN
4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
yes, functions are expression in js
5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
function sayHello(name){
  return `Hello ${name}`
}
6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
hellojohn
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1john

showMessage(); // Output 2hello john

alert(userName); // Output 3john
```

8. What is a Anonymous Function give example of three functions.
let add  = (z,b) = > z+b

9. Can function declaration be a Anonymous Function? Explain
no, in function declaration name of function is required

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
camelcase, start with verb, not an language keyword, start with alphabets only
