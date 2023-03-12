<h1>Steps to understanding the find() method</h1>

<p>The find() method has two arguments which is a callback function and this argument.</p>

find(callback(element[, index[, array]])[, thisArg])

<h2>1. Callback</h2>
<ul>
<li>element is the current element</li>
<li>index of the current element</li>
<li>array that the find() was called upon</li>
<li></li>
</ul>

<h2>2. this argument</h2>

<p>find() - returns the first element in an array that passes a test function.</p>
find(callback(element[, index[, array]])[, thisArg]) find() accepts two arguments one is callback function
and the other one is optional which can be the this inside the callback function.
Example 1:

let users = [
    {id: 1, name: "John"},
    {id: 2, name: "Pete"},
    {id: 3, name: "Mary"},
];

let user = users.find(item => item.id == 2);

alert(user.name); // Pete

Example 2

<p>This example searches for the first even number in an array of numbers:</p>

let numbers = [1, 2, 3, 4, 5];

console.log(numbers.find(e => e % 2 == 0)); //2

Example 3 

<p>Suppose that we have a list of customer objects with name and credit properties as follows:</p>

let customers = [{
    name: 'ABC Inc',
    credit: 100
}, {
    name: 'ACME Corp',
    credit: 200
}, {
    name: 'IoT AG',
    credit: 300
}];

<p>The following code uses the find() method to find the first customer whose credit is greater than 100.</p>

console.log(customers.find(element => element.credit > 100)); //{ name: 'ACME Corp', credit: 200 }

<h1>findIndex()</h1>
 <p>findIndex() is rarely used because it just outputs the index and not the element</p>

 let users =[
  {id: 1, name: "John"},
  {id: 1, name: "Roger"},
  {id: 1, name: "Kelly"},


 ];

 console.log(customers.findIndex(element => element.name == "John"))//0

<h1>lastIndex()</h1>
 

 let users =[
  {id: 1, name: "John"},
  {id: 1, name: "Roger"},
  {id: 1, name: "Kelly"},


 ];

 console.log(customers.lastIndex(element => element.name == "Kelly"))//2