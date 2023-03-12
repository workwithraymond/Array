<h1>How to Manipulate Arrays in Javascript<h1>
Example 1: (how to find the size of the array using the dot notation.)
const movies = ["I am legend", "Lord of The Ring", "John Q"];

console.log(movies.length) //3

Example 2: (This example will show an empty array)

const movies = [];

console.log(movies.length); //0

<h1>How to Access an Array</h1>

<ul>
<li>Each item inside an array is a number called index<li>
<li>Array starts with zero<li>
<li>The names of the elements inside are values<li>
</ul>

Example 3:

const movies = ["Rocky", "Halloween", "Terminator"];

console.log(movies[0]); // rocky
console.log(movies[1]); //Halloween
console.log(movies[2]); //Terminator

<h1>Iterating over an array<h1>

<p>Using a for loop</p>
Example 1

const movies = ["rocky", "Halloween", "Terminator"];

for(let i = 0; i < movies.length; i++) {
    console.log(movies[i]);
}

Example 2

const movies = [1, 4, 5, 6, 7, 8, 9, 3 ];

for(let i = 0; i < movies.length; i ++) {
    console.log(movies[i]);
}

Example 3 (using the forEach)

const numbers = [1, 4, 5, 6, 7, 8, 9, 3];

numbers.forEach(number => {
    console.log(number); //1, 4, 5, 6, 7, 8, 9, 3
});

Example 4 

const numbers = [1, 4, 5, 6, 7, 8, 9, 3];

numbers.forEach(function(i, index) {
    console.log(numbers);
})


Example 5 (using the for-of)

const numbers = [1, 4, 5, 6, 7, 8, 9, 3];

for(const i of numbers) {
    console.log(number)
}

<h1>Adding an element to an array</h1>

Example 1:(adding an element inside an array):

const movies = ["rocky", "Halloween", "Terminator"];

movies.push("ghostbusters")

console.log(moves[3]); // ghostbusters

Example 2: 

const movies = ["rocky", "Halloween", "Terminator"];

movies.push("ghostbusters")

console.log(movies); //"rocky", "Halloween", "Terminator", "ghostbusters"

<p>To add an new element at the beginning use unshift</p>

Example 3: (Adding an new element in the beginning of an array)

const movies = ["rocky", "Halloween", "Terminator", "ghostbusters"]

movies.unshift("Mr. Robot")

console.log(movies); // "Mr.Robot, "rocky", "Halloween", "Terminator", "ghostbusters"

<h1>Removing an element to an array</h1>

Example 4: (Removes the last element of an array)

const movies = ["rocky", "Halloween", "Terminator", "ghostbusters"]

movies.pop() // removes ghostbusters

console.log(movies);//"rocky", "Halloween", "Terminator"

Example 5: (Using splice which has two parameters first one is the index from which
to begin removing, and second one is the number of elements to remove).

const movies = ['rocky', 'Halloween', 'Terminator', 'ghostbusters']

movies.splice(0,1) //removes rocky

console.log(movies); //'Halloween', 'Terminator', 'ghostbusters'

<p>Another example for splice()</p>

let movies = ['rocky', 'Halloween', 'Terminator', 'ghostbusters']
movies.splice(2, 1) // removes terminator
console.log(movies)// 'rocky', 'Halloween', 'ghostbusters'

<p>Another example for splice()</p>

let movies = ['rocky', 'Halloween', 'Terminator', 'ghostbusters', 'Avengers', 'honor']

movies.splice(2, 2, 'code', 'glory') // remove Terminator and ghostbusters and add code and glory


Example 6: (Using shift() Takes out an item from the beginning)

const movies = ['Halloween', 'Terminator', 'ghostbuster', 'rocky']

movies.shift()

console.log(movies); // 'Terminator', 'ghostbuster', 'rocky'

Example 7: (Using Slice) this returns a new array copying to it all items from index
start to end (not including end)

let fruits = ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango']
fruits.slice(1, 4) 

console.log(fruits);//'Orange', 'Lemon', 'Apple'


var array=[1,2,3,4,5]
console.log(array.slice(2));
// shows [3, 4, 5], returned selected element(s).
 
console.log(array.slice(-2));
// shows [4, 5], returned selected element(s).
console.log(array);
// shows [1, 2, 3, 4, 5], original array remains intact.
 
var array2=[6,7,8,9,0];
console.log(array2.slice(2,4));
// shows [8, 9]
 
console.log(array2.slice(-2,4));
// shows [9]
 
console.log(array2.slice(-3,-1));
// shows [8, 9]
 
console.log(array2);
// shows [6, 7, 8, 9, 0]

<h1>Adding concat() into an array.  What this does is it merges two or more arrays</h1>

const array1 = ['a', 'b', 'c'];
const array2 = ['d', 'e', 'f'];
const array3 = array1.concat(array2);
console.log(array3);

<h1>Searching in Array</h1> 
<p>indexOf - looks for items starting from index from, and returns the index where it was
found, otherwise -1. </p>

let fruits = ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango']

console.log(fruits.indexOf('Orange'));//1
console.log(fruits.indexOf('Lemon')); //2
console.log(fruits.indexOf('pepper')); // -1 because its not in the array

<p>include()- if the element is in the array than its going to say true if not in the array
its going to result in false</p>

let fruits = ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango']

console.log(fruits.include('Orange'));//true
console.log(fruits.include('plum'));//false

<h1>Using the reverse() method</h1>

let arr = [1,2,3,4,5,6,7,8];
arr.reverse();
alert(arr);//8,7,6,5,4,3,2,1

<h1>split()</h1>

<p>This splits the string into an array by the given delimiter.</p>

let names = 'Bilbo', Gandalf, Nazgul';

let arr = names.split(', ');

for (let name of arr) {
    alert(`A message to ${name}.` ); //A message to Bilbo 
}

Example 2:  splits into letters

let str = "test";

alert( str.split('') ); //t,e,s,t

<h1></h1>



