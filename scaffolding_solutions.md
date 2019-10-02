1. Write a program that ask the user for a number and tells the user whether it's:
(a) odd or even; (b) positive, negative, or neither; (c) an integer.

```javascript

let number = prompt("Enter a number");
if (number % 2 == 0) {
  alert("Your number is even");
} else {
  alert("Your number is odd");
}
if (number > 0) {
  alert("Your number is positive");
} else if (number < 0) {
  alert("Your number is negative");
} else {
  alert("Your number is neither positive nor negative");
}
if (number == Math.floor(number)) {
  alert("Your number is an integer");
} else {
  alert("Your number is not an integer");
}
```

2. Write a program that asks the user to enter numbers and keeps (and displays) the running total
of these numbers.

```javascript
let total = 0;
while (true) {
  let number = prompt("Enter the next number");
  total += Number(number);
  alert("The running total is "+total);
}
```

3. Define a function `CtoF()` that converts temperature from Celsius to Fahrenheit.

```javascript
const CtoF = function(C) {
  let F = C * (9/5) + 32;
  return F;
}
```


4. Define a function that uses recursion calculates the Fibonacci number *F(n)* for any given natural number *n* as follows: F(1)=1, F(2)=1, F(n)=F(n-2)+F(n-1).

```javascript
const fibonacci = function(n) {
  if (n == 1 || n == 2) return 1;
  return fibonacci(n-2) + fibonacci(n-1);
}
```
