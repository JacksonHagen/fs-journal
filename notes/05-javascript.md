# JavaScript

let = local scope variable
var = global score variable
const = constant - cannot reassign

let obj = {name: "jack"}
let obj2 = {name: "jack"}

obj == obj //RETURNS TRUE
//compares memory addresses

obj == obj2 //RETURNS FALSE
//compares memory addresses

<br>

[] Is bracket notation. It refers to indices. Works on dictionaries and arrays. Can any datatype within
#### ACCESS A PROPERTY OF AN OBJECT USING A VARIABLE WITH BRACKET NOTATION

let atr = attribute

obj[atr] = obj.attribute

<br>

A parameter is the content that needs to be passed into a function
An argument is the contents of the variable that is being passed as a parameter to a function

originalArray.filter(arrayItem => arrayItem === condition) Returns a new array of true values from originalArray

array.forEach(arr => {
     loop contents here
}) 
array.forEach iterates over each item in an array and executes code after
