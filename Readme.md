# Full name printer

Write the implementation of `printFullName()`, which Pprints the full name of a person

```javascript
// function printFullName(firstName, lastName)
printFullName("Amr", "Elsekilly");

// output
/*
Amr Elsekilly
*/
```

# Age Calculator

Write the implementation of `ageToToday()`, which calculates your age till today.

```javascript
// function ageToToday(day, month, year)
ageToToday(24, 6, 1993);

// output
/*
Age:
26 years 11 months 21 days
or 323 months 21 days
or 1407 weeks 3 days
or 9,852 days
or 236,448 hours
or 14,186,880 minutes
or 851,212,800 seconds
*/
```

# Capitalization

Write the implimentation of `capitalizeString()`, which capitalizes the first letter of any string at the beginning of the sentence and after the dots (full-stop).

```javascript
// function capitalizeString(string)
capitalizeString("hello world!");

// output
/*
Hello world!
*/

capitalizeString("hello world. it's a lovely day. i should go out");

// output
/*
Hello world. It's a lovely day. I should go out
*/
```

# Oddish vs. Evenish

Create a function that determines whether a number is Oddish or Evenish. A number is Oddish if the sum of all of its digits is odd, and a number is Evenish if the sum of all of its digits is even. If a number is Oddish, return "Oddish". Otherwise, return "Evenish".

For example, oddishOrEvenish(121) should return "Evenish", since 1 + 2 + 1 = 4. oddishOrEvenish(41) should return "Oddish", since 4 + 1 = 5.

```javascript
oddishOrEvenish(43) ➞ "Oddish"

oddishOrEvenish(373) ➞ "Oddish"

oddishOrEvenish(4433) ➞ "Evenish"
```

# Seven Boom!

Create a function that takes an array of numbers and return "Boom!" if the number 7 appears in the array. Otherwise, return "there is no 7 in the array".

```javascript
sevenBoom([1, 2, 3, 4, 5, 6, 7]) ➞ "Boom!"

sevenBoom([8, 6, 33, 100]) ➞ "there is no 7 in the array"

sevenBoom([2, 55, 60, 97, 86]) ➞ "Boom!"
```

# Count Number of Identical Arrays

Create a function that takes four arrays as arguments and returns a count of the total number of identical arrays.

```javascript
countIdenticalArrays([0, 0, 0], [0, 1, 2], [0, 0, 0], [2, 1, 0]) ➞ 2

countIdenticalArrays([0, 1, 0], [0, 1, 2], [0, 2, 0], [2, 1, 0]) ➞ 0

countIdenticalArrays([0, 1, 2], [0, 1, 2], [0, 1, 2], [2, 1, 0]) ➞ 3
```

# How Many Days Between Two Dates

Create a function that takes two dates and returns the number of days between the first and second date.

```javascript 
getDays(
  new Date("June 14, 2019"),
  new Date("June 20, 2019")
) ➞ 6

getDays(
  new Date("December 29, 2018"),
  new Date("January 1, 2019")
) ➞ 3

getDays(
  new Date("July 20, 2019"),
  new Date("July 30, 2019")
) ➞ 10
```

# Hard Problems

# Reversing a Binary String

Write a function that takes an integer n, reverses the binary representation of that integer, and returns the new integer from the reversed binary.

```javascript
reversedBinaryInteger(10) ➞ 5
// 10 = 1010 -> 0101 = 5

reversedBinaryInteger(12) ➞ 3
// 12 = 1100 -> 0011 = 3

reversedBinaryInteger(25) ➞ 19
// 25 = 11001 -> 10011 = 19

reversedBinaryInteger(45) ➞ 45
// 45 = 101101 -> 101101 = 45
```

# Valid Name

For this exercise, keep in mind the following definitions:

A term is either an initials or word.
initials = 1 character
words = 2+ characters (no dots allowed)
A valid name is a name written in one of the following ways:

H. Wells
H. G. Wells
Herbert G. Wells
Herbert George Wells
The following names are invalid:

Herbert or Wells (single names not allowed)
H Wells or H. G Wells (initials must end with dot)
h. Wells or H. wells or h. g. Wells (incorrect capitalization)
H. George Wells (middle name expanded, while first still left as initial)
H. G. W. (last name is not a word)
Herb. G. Wells (dot only allowed after initial, not word)

## Rules
- Both initials and words must be capitalized.
- Initials must end with a dot.
- A name must be either 2 or 3 terms long.
- If the name is 3 words long, you can expand the first and middle name or expand the first - name only. You cannot keep the first name as an initial and expand the middle name only.
- The last name must be a word (not an initial).
- Your task is to write a function that determines whether a name is valid or not. Return true if the name is valid, false otherwise.

```javascript
validName("H. Wells") ➞ true

validName("H. G. Wells") ➞ true

validName("Herbert G. Wells") ➞ true

validName("Herbert") ➞ false
// Must be 2 or 3 words

validName("h. Wells") ➞ false
// Incorrect capitalization

validName("H Wells") ➞ false
// Missing dot after initial

validName("H. George Wells") ➞ false
// Cannot have: initial first name + word middle name

validName("H. George W.") ➞ false
// Last name cannot be initial

validName("Herb. George Wells") ➞ false
// Words cannot end with a dot (only initials can)
```

# Time Elapsed

Create a function that takes two timestamps as input, and returns a string describing the time elapsed between them (in days, hours, minutes, seconds as appropriate).

Note: Timestamps are seconds elapsed since 1st January 1970.

```javascript
elapsed(1559813526, 1559899926) ➞ "1 day"

elapsed(1559681004, 1559899926) ➞ "2 days, 12 hours, 48 minutes, 42 seconds"

elapsed(1558773066, 1559899926) ➞ "13 days, 1 hour, 1 minute"
```