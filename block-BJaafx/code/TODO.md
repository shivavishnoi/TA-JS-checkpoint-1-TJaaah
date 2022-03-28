1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let sum = 0
for(let i = 1; i<=10; i++){
   sum += +prompt(`enter number`)
}
console.log(sum, sum/10)
```
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
hi hi hi

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
let sum = 0
function getEvenSum(max=10){
  for (i=1; i<=max; i++){
    if(i%2==0){
        sum += i
    }
  }
}
```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
let sum = 0
function getEvenSum(max=10){
  for (i=1; i<=max; i++){
    if(i%2 !=0){
        sum += i
    }
  }
}
```
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.
```js
function getProductOfDigits(num){
  if(num<=0){
    return `not valid`
  }
  num = String(num)
  let product = 1
  for(let i=0; i< num.length; i++){
     product *= Number(num[i])
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

check(10); // output bigger than 5
check(1); // output  smaller than 5
check(5); // output  5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // what will be the output arya
getOutput('John'); // what will be the output john 
getOutput(); // what will be the output  who are u, because no parameter passed to name argument thus it will be undefined, and function has a return statement which will execute
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // what will be the output
getOutput('John'); // what will be the output
getOutput(); // what will be the output who are you
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
A funtion can use only one return statemen, but within conditions we can give multiple return statement
```js
function a(num==10){
  if(num==10){
    return true
  }
  else{
    return false
  }
}
```
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
for loop  is used when we have a definite range, whereas while loop is used when steps should be repeated until a condition is satisfied
