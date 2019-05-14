# ENGL 516 - Methods of Formal Linguistic Analysis

**Textbook (required):** [Eloquent Javascript, 3rd edition](https://eloquentjavascript.net/) by Marijn Haverbeke. There is a free online version and a [paperback](https://www.amazon.com/Eloquent-JavaScript-3rd-Introduction-Programming/dp/1593279507/) for $25.

## Schedule

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

## Course Assessment Plan

- Five small projects (A-E): 5% each, 25% total (rubric provided on the assignment sheet for each small project)
- Oral exam based on the small projects: 25% (rubric provided on the study guide)
- Final project: 30% (rubric provided on the assignment sheet)
- Written final exam: 20% (rubric provided on the study guide)

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

- Your program (prompt box): `Is your number 23?`
- User (enters into the prompt box): `<`
- Your program: `Is your number 1?`
- User: `>`
- Your program (prompt box): `Is your number 14?`
- User (enters into the prompt box): `yes`
- Your program (alert box): `I won!`

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

- Your program: `Enter shift`
- User: `-5`
- Your rprogram: `Enter text`
- User: `Hello, world!`
- Your program: `Czggj, rjmgy!`

**Note:** The wording of the prompts "Enter shift" and "Enter text" is not
prescribed, but the sequence of prompt boxes must follow the task
description.

#### Grading (5 points total)

- Your is syntactically correct: 1 point
- Your program correctly encodes strings that I supply: 4 points

### Small Project C: Learner Modeling

**Learning outcome:** After completing this assignment, you will have learned how to model
language learning goals and the current state of language learner using data structures (objects
and arrays) in JavaScript. You will also learn how to develop simple adaptive computer-assisted
language learning algorithms.

**Programming concepts:** array, object, random.

#### Task

Write a program that teaches English prepositions using a series of fill-in-the-blank exercises. Each
exercise will be in the following format:

`Are you wearing anything ___ your sweater?`

That is, the exercise will have a sentence with a preposition replaced with a sequence of underscores.
The user of your program will be an English language learner. The user will complete each exercise by
entering the preposition which, in the user's opinion, should be inserted in place of the blank. For example,
a response to the exercise shown above might be:

`underneath`

Your program will show each exercise in a prompt box. After the user enters their response, your program will display
an alert box which can have one of the following two messages:

- a message saying `Correct!` if the user's response was correct; or
- a message displaying the sentence with the correct preposition, for example: `Are you wearing anything underneath your sweater?`

After presenting this feedback to the user, the program will  move on to displaying the next exercise.

Your program will be tracking the user's progress in the learning of each preposition. At each step, the program
will provide an exercise targeting the preposition which the user has mastered to the least extent. Mastery level
for the preposition *x* should be calculated as the number of times the user has gotten the preposition *x* correct
in exercises less the number of times the user has gotten the preposition *x* wrong.

You should use a JavaScript object in your program to track the user's mastery levels for all prepositions.

You should develop your program so that it supports at least five different prepositions and provides at least
five different exercises for each preposition that your program supports.

#### Sample input/output

- Your program (prompt box): `There is a table ___ the room.`
- User (enters into prompt box): `on`
- Your program (alert box): `There is a table in the room.`
- Your program (prompt box): `The train will arrive ___ two hours.`
- User: `in`
- Your program: `Correct!`

#### Grading (5 points total)

- Your program is syntactically correct: 1 point.
- Your program supports 5 prepositions, and for each preposition it supports 5 possible sentences: 1 point.
- Your program implements a tutoring algorithm consisent with the assignment: 3 points.

### Small Project D: Haigy Paigy

**Learning outcome:** Through completing this assignment, you will learn to
use regular expressions in JavaScript to perform search and replace operations on strings.
You will also learn to "translate" conceptual definitions of applied linguistic problems into
formal instructions that are programmable for the computer.

**Programming concepts:** regular expressions.

#### Task

Haigy Paigy is as a children's invented language which sounds exactly like English, except that "aig" is inserted before
the rime of each syllable. E.g., the English word "hello" becomes "haigellaigo" in Haigy Paigy.

Write a program in JavaScript that will prompt the user to enter a sentence, automatically translate it from English
into Haigy Paigy, and display the result of the translation as an alert box. In your program, you will need to write
a set of regular expressions that will translate the input sentence into Haigy Paigy.

**Simplifications:** only vowels can be syllable nuclei; the letter "y" always makes a vowel sound; several consecutive
vowel letters always make a single vowel sound; the final "e" is always silent, except when it is the only vowel letter
in the word.

#### Sample input/output

User: `This is a test.`
Your program: `Thaigis aigis aiga taigest.`

#### Grading (5 points total)

- Your is syntactically correct: 1 point
- Your program correctly translates sentences that I supply: 4 points
