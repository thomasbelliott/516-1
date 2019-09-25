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

```
let total = 0;
while (true) {
  let number = prompt("Enter the next number");
  total += number;
  alert("The running total is "+total);
}
```