# ca-arrays-secret-message(s) and other array methods

Objective
## LEARN JAVASCRIPT  - Coding Methods

Docs here : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#Iteration_methods

### Secret Message
Using array methods, you will transform an array of strings into a secret message!
You should consult the *Mozilla Developer Network (MDN)* 
for reference on any method with which you are not familiar.


### The .map() Method
The second iterator we’re going to cover is .map(). When .map() is called on an array, it takes an argument of a callback function and returns a new array! Take a look at an example of calling .map():

>const numbers = [1, 2, 3, 4, 5]; 
 
>const bigNumbers = numbers.map(number => {
  return number * 10;
>});
>.map() works in a similar manner to .forEach()— the major difference is that .map() returns a new array.
>

visit here for the coding solution:
https://gist.github.com/5701205819e719608bf44438fc107f2c


### The .filter() Method
Another useful iterator method is .filter(). Like .map(), .filter() returns a new array. However, .filter() returns an array of elements after filtering out certain elements from the original array. The callback function for the .filter() method should return true or false depending on the element that is passed to it. The elements that cause the callback function to return true are added to the new array. Take a look at the following example:

.
>const words = ['chair', 'music', 'pillow', 'brick', 'pen', 'door']; 
 
>const shortWords = words.filter(word => {
>  return word.length < 6;
>});
>
visit here for the coding solution:
https://gist.github.com/f56795e2e52e0698621f9d7f6ec9911c


### The .findIndex() Method
We sometimes want to find the location of an element in an array. That’s where the .findIndex() method comes in! Calling .findIndex() on an array will return the index of the first element that evaluates to true in the callback function.

>const jumbledNums = [123, 25, 78, 5, 9]; 
 
>const lessThanTen = jumbledNums.findIndex(num => {
>  return num < 10;
> });
jumbledNums is an array that contains elements that are numbers.
const lessThanTen = declares a new variable that stores the returned index number from invoking .findIndex().
The callback function is an arrow function has a single parameter, num. Each element in the jumbledNums array will be passed to this function as an argument.
num < 10; is the condition that elements are checked against. .findIndex() will return the index of the first element which evaluates to true for that condition.

visit here for the coding solution:
https://gist.github.com/f853dc34535c377508e585c1cb5d4e52


### The .reduce() Method
Another widely used iteration method is .reduce(). The .reduce() method returns a single value after iterating through the elements of an array, thereby reducing the array. Take a look at the example below:

>const numbers = [1, 2, 4, 10];
 
>const summedNums = numbers.reduce((accumulator, currentValue) => {
> return accumulator + currentValue
> })
 
> console.log(summedNums) // Output: 17
> Here are the values of accumulator and currentValue as we iterate through the numbers array:

visit here for the coding solution:
https://gist.github.com/f75160385128495fb7dfe3db74707dae

### Iterator Documentation
There are many additional built-in array methods, a complete list of which is on the MDN’s Array iteration methods page.

The documentation for each method contains several sections:

A short definition.
A block with the correct syntax for using the method.
A list of parameters the method accepts or requires.
The return value of the function.
An extended description.
Examples of the method’s use.
Other additional information.

visit here for the coding solution:
https://gist.github.com/fad7217f6202efcb190cb80e636b9c72
