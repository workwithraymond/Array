<p>Array.map creates a new array</p>

Example 1:

let num = [3, 4, 5, 6];

let modifiedArr = num.map(function(element) {
    return element * 3;
    });

console.log(modifiedArr); //9, 12, 15, 18

Example 2:

let users = [
    {firstName : 'Raymond', lastName : 'Del Rosario'},
    {firstName : 'John',  lastName : 'Rodriguez'},
    {firstName : 'Roger', lastName : 'Campbell'}
];

let userFullNames = users.map(function(element) {
    return `${element.firstName} ${element.lastName}`;
})

console.log(userFullNames);//'Raymond Del Rosario', 'John Rodriguez', 'Roger Campbell'

Example 3:

let lengths = ['limbo', 'box', 'data', 'dreaming'].map(item => item.length);
alert(lengths)