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
