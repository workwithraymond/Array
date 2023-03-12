<p>the filter() method is used to create a new array from a given array consisting of only those elements
from the given array which satify a condition set by the argument method</p>

array.filter(callback(element, index, arr), thisValue)

<ul>
    <li>callback</li>
    <li>element</li>
    <li>index</li>
    <li>arr</li>
    <li>thisValue</li>
</ul>
Example 1:

let users = [
    {id: 1, name: 'john'},
    {id: 2, name: 'robert'},
    {id: 3, name: 'kenny'},
    {id: 4, name: 'raymond'}
];

let someUsers = users.filter(user => this.id < 3); 

console.log(users.length);//2

<p>Example 2:  In this example, the method filter() creates a new array consisting of only those elements that satisfy the condition checked by canVote() function.</p>

function canVote(age){
    return age >= 18;
}

function ageLimit() {
    let result = [23, 45, 21, 18, 16, 30].filter(canVote);
    console.log(result);
}
ageLimit();//23,45,21,30

Example 3

<p> In this example, the method filter() creates a new array consisting of only those elements that satisfy the condition checked by isPositive() function.</p>

function isPositive(value) {
    return value > 0;
}

let newPositive = [2, 5, 6, -1, -3].filter(isPositive)
console.log(newPositive);//2, 5, 6

Example 4

<p>In this example, the method filter() creates a new array consisting of only those elements that satisfy the condition checked by isEven() function. </p>

 function isEven(value) {
      return value % 2 == 0;
    }

    












