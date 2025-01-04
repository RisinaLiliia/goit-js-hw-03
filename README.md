# goit-js-hw-02

Task 1. Slug Generator

Perform this task in the file task-1.js

Before solving the task, let's define a new term!

The term slug is a human-readable unique identifier used in web development to create readable URLs.

For example, instead of the user seeing mysite.com/posts/1q8fh74tx in the address bar, you can make a slug from the title of the article. As a result, the address will be more pleasant to perceive: mysite.com/posts/arrays-for-beginners.

A slug is always a lowercase string, the words of which are separated by dashes.

Did you figure it out? Now let's finally do the task!

Write a function slugify(title) that takes the title of the article, the title parameter, and returns a slug created from this string.

The value of the title parameter will be strings whose words are separated only by spaces.
All slug characters must be lowercase.
All slug words must be separated by dashes.
Take the code below and paste it after the declaration of your function to verify that it works correctly. The results of its operation will be displayed in the console.

console.log(slugify("Arrays for beginners")); // "arrays-for-beginners"
console.log(slugify("English for developer")); // "english-for-developer"
console.log(slugify("Ten secrets of JavaScript")); // "ten-secrets-of-javascript"
console.log(slugify("How to become a JUNIOR developer in TWO WEEKS")); // "how-to-become-a-junior-developer-in-two-weeks"

Leave this code for review by a mentor.

What the mentor will pay attention to when checking:

Declared function slugify(title)
Calling slugify("Arrays for beginners") returns "arrays-for-beginners"
Calling slugify("English for developer") returns "english-for-developer"
Calling slugify("Ten secrets of JavaScript") returns "ten-secrets-of-javascript"
Calling slugify("How to become a JUNIOR developer in TWO WEEKS") returns "how-to-become-a-junior-developer-in-two-weeks"

Task 2. Array composition

Perform this task in the file task-2.js

Write a function called makeArray that takes three parameters: firstArray (array), secondArray (array), and maxLength (number). The function should create a new array that contains all the elements from firstArray, and then all the elements from secondArray.

If the number of elements in the new array exceeds maxLength, the function should return a copy of the array with the length of maxLength of elements.
Otherwise, the function should return the entire new array.

Take the code below and paste it after the declaration of your function to verify that it works correctly. The results of its operation will be printed to the console.

console.log(makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)); // ["Mango", "Poly", "Ajax"]
console.log(makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)); // ["Mango", "Poly", "Houston", "Ajax"]
console.log(makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)); // ["Mango", "Ajax", "Chelsea"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)); // ["Earth", "Jupiter"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)); // ["Earth", "Jupiter", "Neptune", "Uranus"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)); // []

Leave this code for review by a mentor.

What the mentor will pay attention to when checking:

Declared function makeArray(firstArray, secondArray, maxLength)
Call makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3) returns ["Mango", "Poly", "Ajax"]
Call makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4) returns ["Mango", "Poly", "Houston", "Ajax"]
Call makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3) returns ["Mango", "Ajax", "Chelsea"]
Call makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2) returns ["Earth", "Jupiter"]
Call makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4) returns ["Earth", "Jupiter", "Neptune", "Uranus"]
Calling makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0) returns []
Calling makeArray() with random arrays and a random number returns the correct array

Task 3. Filtering an array of numbers

Perform this task in the file task-3.js

Write a function filterArray(numbers, value) that takes an array of numbers and a value as parameters. The function should return a new array of only those numbers from the numbers array that are greater than the value value.

Inside the function:

Create an empty array to which you will add the matching numbers.
Use a loop to iterate over each element of the numbers array.
Use an if statement inside the loop to test each element and add it to your array.
Return your new array with the matching numbers as the result.

Take the code below and paste it after the declaration of your function to verify that it works correctly. The results of its operation will be printed to the console.

console.log(filterArray([1, 2, 3, 4, 5], 3)); // [4, 5]
console.log(filterArray([1, 2, 3, 4, 5], 4)); // [5]
console.log(filterArray([1, 2, 3, 4, 5], 5)); // []
console.log(filterArray([12, 24, 8, 41, 76], 38)); // [41, 76]
console.log(filterArray([12, 24, 8, 41, 76], 20)); // [24, 41, 76]

Leave this code for review by a mentor.

What the mentor will pay attention to when checking:

The declared function filterArray(numbers, value)
Calling the function filterArray([1, 2, 3, 4, 5], 3) returns [4, 5]
Calling the function filterArray([1, 2, 3, 4, 5], 4) returns [5]
Calling the function filterArray([1, 2, 3, 4, 5], 5) returns []
Calling the function filterArray([12, 24, 8, 41, 76], 38) returns [41, 76]
Calling the function filterArray([12, 24, 8, 41, 76], 20) returns [24, 41, 76]
Calling the function filterArray() with a random array and a number returns the correct array
