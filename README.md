# Array Iteration Methods Lab

## Learning Goals

* Practice using `filter()` to return matching results
* Practice using `find()` to isolate a specific result
* Practice using `forEach()` to directly change array elements

## Introduction

Now that we've learned about some array iteration methods, it's time to practice 
using them. In this lab, you'll write functions that use the `filter()` `find()`
and `forEach()` methods. 

If you haven't already, fork and clone this lab into your local environment. Navigate into 
its directory in the terminal, then run `code .` to open the files in Visual Studio Code.
Do your work in the `index.js` file.

Install all the dependencies with npm install to ensure you can test your work as you 
go with `npm test`.

## Instructions

**Use `filter()` to Return Matching Results**

We have an array of drivers with various information. We need to write a function
using the `filter()` method so that PickMeUp Taxi service employees can easily
query the data. Run the tests to see what conditions need to be met by each
function _before_ you start writing JavaScript code.

You'll be writing the function:

* `findMatching`- This function takes an array of drivers' names and the name
  to search for as arguments, and returns the matching list of drivers. The function 
  should be case insensitive.

**Use `find()` to Isolate a Specific Result**

We have an array of a football's teams record in the Superbowl. We need to
create a function that uses the `find()` method to single out a specific
result in the record data for the Denver Broncos. We want to find out if, at _any_ 
point in the team's existence, they've had a win in the Superbowl. Our data looks 
like this:

```js
const record = [
  { year: "2015", result: "W"},
  { year: "2014", result: "N/A"},
  { year: "2013", result: "L"},
  //...
]
```

You'll be writing the function:

* `superbowlWin()` - This function takes an array of objects as shown above, and 
  returns a year the Denver Broncos won the superbowl. In other words, it should
  return a year where the `result` is `"W"`. If no win is found, it should return,
  sadly, `undefined`

**Use `forEach()` to Directly Manipulate Array Elements**

We have an array of people that gives us their name and birth year. We need to write
a function that will calculate their current age and add it as a property on the 
person's object. Our data originally looks like this:

```js
const people = [
  { name: "Meredith", birthYear: 1985 },
  { name: "Hasung", birthYear: 1994 },
  { name: "Julio", birthYear: 1963 }
]
```

After running it through the function you write, it should look like this (assuming the
current year is 2022):

```js
[
  { name: "Meredith", birthYear: 1985, currentAge: 37 },
  { name: "Hasung", birthYear: 1994, currentAge: 28 },
  { name: "Julio", birthYear: 1963,  currentAge: 59 }
]
```

You'll be writing the function:

* `addCurrentAge()` - This function takes an array of people as shown above and 
  the current year, and adds a `currentAge` property to each person's object. The
  age should be calculated from the year passed in and the person's birth year.

## Resources

* [MDN: Array.prototype.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)
* [MDN: Array.prototype.find()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find)