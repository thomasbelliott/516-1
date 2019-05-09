# ENGL 516 - Methods of Formal Linguistic Analysis

**Textbook (required):** [Eloquent Javascript, 3rd edition](https://eloquentjavascript.net/) by Marijn Haverbeke. There is a free online version and a [paperback](https://www.amazon.com/Eloquent-JavaScript-3rd-Introduction-Programming/dp/1593279507/) for $25.

## Schedule:

- W1: Foundations of information theory. Numeral systems.
- W2: Representing logic, numbers, text, colors, and sounds in the computer.
- W3: Chapter 1: Values, types, and operators. Exercises.
- W4: Chapter 2: Program structure.
- W5: Small Project A: Number Guessing Game (5%).
- W6: Chapter 3: Functions.
- W7: Small Project B: Caesar Cipher (5%).
- W8: Chapter 4: Data structures: objects and arrays.
- W9: Small Project C: Learner Modeling (5%).
- W10: Chapter 9: Regular expressions.
- W11: Small Project D: Haigy Paigy (5%).
- W12: Small Project E: Corpus Processing (5%).
- W13: Oral exam - 25% - based strictly on Small Projects A-E.
- W14: Chapter 13: JavaScript and the Browser.
- W15: Final Project Presentations (Final project worth 30%).
- Finals week: Written final exam (worth 20%).

(For W1 & W2, read the Introduction from the textbook.)

## Assignment Sheets

### General Notes

#### Submission deadlines

Each small project is due by the end of day on Wednesday following the week when the project is assigned.
Grades will be given by the end of day on Friday of the week when the project is due.
Formative feedback will be provided by the end of day on Wednesday of the following week.
To keep you on track with the class, late submissions are strongly discouraged. If you must submit a small project late,
you must tell me in advance.

#### Submission procedure

I will access your GitHub
repository after the deadline to retrieve your project file. For each small project, create a new file
in your GitHub repository named **projectx.html**, where **x** is the letter designation of the project (**a**-**e**).
Your file name should not contain quotes, spaces,
or any other symbols. Please also note that file names are case sensitive,
so "PROJECTA.HTML" and "projecta.html" are two different files. After you
complete your assignment, do not forget to "commit master" and "push
origin". Make sure that your program carefully follows the input/output protocol described in the assignment directios.

### Small Project A: Number Guessing Game

**Learning outcome:** After completing this assignment, you will have learned how to
conceptualize and implement in code a simple algorithm. Algorithms are a
foundation of computer science and computational linguistics. The algorithm
used in this small project is widely used in applied
linguistics. For example, it is one of the primary alrogithms used in
adaptive computer-assisted language testing.

**Programming concepts:** while-loop, binding, string, number, string comparison, condition.

#### Task

Create a web page with an embedded JavaScript program that plays the
"number guessing game" with the user as follows:

1. The user is asked to think of an integer number between 1 and 100 (inclusive).
2. The program needs to repeatedly take guesses at the number the user has in mind.
3. To each of the program's guesses, the user responds "<" if the target
number is less than the program's guess; ">" if the target number is
greater than the program’s guess; or "yes" if the program has guessed the
number correctly.

You need to come up with and implement the most efficient strategy for your
program.

#### Sample game

- Your program (prompt box): Is your number 23?
- User (enters into the prompt box): <
- Your program: Is your number 1?
- User: >
- Your program (prompt box): Is your number 14?
- User (enters into the prompt box): yes
- Your program (alert box): I won!

#### Grading (5 points total)

- Your program is syntactically correct: 1 point.
- Your program is able to guess numbers: 1 point.
- Your program guesses numbers in the most efficient way: 3 points.

### Small Project B: Caesar Cipher

**Learning outcome:** After completing this assignment, you will have learned how to process
strings of text on a character-by-character level, how to extract
characters from strings, how to concatenate strings, and how to convert
characters to their ASCII codes and back.

**Programming concepts:** for-loop, string, character, ASCII code, modular arithmetic.

#### Task

Create a web page with an embedded JavaScript program that implements
Caesar cipher with a user-specified shift for the upper-case and lower-case
English letters. The letters must wrap around.

1. The user is shown a first prompt box and asked to enter a positive or
negative integer number representing the desired shift. For example, a left
shift of 3 places would be represented as -3; a right shift of 1 place
would be represented as 1.

2. The user is shown a second prompt box, asking to enter the source
(unencrypted) text.

3. The user is shown an alert box with the encrypted text.

In the encryption process, only letters A-Z and a-z are encoded; other
characters must be left untouched.

#### Sample input/output

- Your program: Enter shift
- User: -5
- Your rprogram: Enter text
- User: Hello, world!
- Your program: Czggj, rjmgy!

**Note:** The wording of the prompts "Enter shift" and "Enter text" is not
prescribed, but the sequence of prompt boxes must follow the task
description.

#### Grading (5 points total)

- Your is syntactically correct: 1 point
- Your program correctly encodes strings that I supply: 4 points
