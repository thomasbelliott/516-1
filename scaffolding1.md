**Problem #1. Write a program that asks the user to enter two numbers and displays an alert box with the sum of the numbers entered.**

<details><summary>Solution #1</summary>
<p>

```javascript
let a = prompt("Enter one number");
let b = prompt("Enter another number");
let c = parseFloat(a) + parseFloat(b);
alert("The sum is "+c);
```

</p>
</details>

**Problem #2. Write a program that asks the user for the distance in feet and converts it to meters.**

<details><summary>Solution #2</summary>
<p>

```javascript
let feet = prompt("Enter distance in feet");
let meters = feet / 3.281;
alert("The distance is meters "+meters);
```

</p>
</details>

**Problem #3. Write a program that asks the user to enter a year and then tells the user if this year is a leap year. See [Leap year in the Gregorian calendar](https://en.wikipedia.org/wiki/Leap_year#Gregorian_calendar)**

<details><summary>Solution #3</summary>
<p>
  
```javascript
let year = prompt("Enter year number");
let is_leap;
if (year % 4 != 0) {
  is_leap = false;
} else if (year % 100 != 0) {
  is_leap = true;
} else if (year % 400 != 0) {
  is_leap = false;
} else {
  is_leap = true;
}

if (is_leap) {
  alert("The year "+year+" is a leap year");
} else {
  alert("The year "+year+" is a common year");
}
```

More concise:

```javascript
let year = prompt("Enter year number");
// using the fact that 0 is falsey and any other number is truthy
let is_leap = year % 4 ? 0 : year % 100 ? 1 : year % 400 ? 0 : 1;
alert("The year "+year+" is a "+(is_leap ? "leap" : "common")+" year");
```

</p>
</details>

**Problem #4. Write a program that asks the user to enter numbers a, b, c and then calculates the roots x<sub>1</sub> and x<sub>2</sub> of the quadratic equation ax<sup>2</sup> + bx + c = 0. Use the [quadratic formula](https://en.wikipedia.org/wiki/Quadratic_formula) in your program, but also handle the cases when there are no real roots (i.e. the discriminant is less than 0), there is only one root (i.e. the discriminant is equal to zero), and the equation is linear (i.e. a = 0).**

<details><summary>Solution #4</summary>
<p>
  
```javascript
let a = parseFloat(prompt("Enter a"));
let b = parseFloat(prompt("Enter b"));
let c = parseFloat(prompt("Enter c"));

if (a == 0) {
  if (b == 0) {
    alert("There are no roots");
  } else {
    let x = -c/b;
    alert("This is a linear equation. x="+x);
  }
} else {
  let d = b * b - 4 * a * c;
  if (d > 0) {
    let x1 = (-b + sqrt(d)) / (2 * a);
    let x2 = (-b - sqrt(d)) / (2 * a);
    alert("There are two roots: x1="+x1+"; x2="+x2);
  } else if (d == 0) {
    let x = -b / (2 * a);
    alert("There is only one root: x="+x);
  } else {
    alert("There are no real roots");
  }
} 
  
```

</p></details>
