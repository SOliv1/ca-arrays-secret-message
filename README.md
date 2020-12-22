# ca-arrays-secret-message(s)

Objective
## LEARN JAVASCRIPT  - Coding Methods

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
