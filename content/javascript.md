+++
title = 'Javascript'
date = 2023-09-27T09:21:26+07:00
draft = true
+++

# Variable
- declaring variable
	- `const varname`
		- top level object cant change
		- *but object member variable CAN change*
	- `let varname`
		- use this, dont use var
- get variable type
	- `console.log(typeof varname)`
- variable operation
	- string concat
		- `let newstring = 'Age is' + 20)`
		- ```let newstring = `${"Age is"} ${25}` ```
- array
	- can be multiple types in one
	- `let array = ["Hello", 10, 3.14, {name: "John"}]`
	- get array length
	- `console.log(array.length)`

# Object
- declaring
	- `let object = {key1: 'value', key2: 'value2', key3: 'value3'}`
- get value of a key
	- `console.log(object["key"])`
	- `console.log(x.key)`
- override key value
	- `object.key1 = 'newvalue1'`
	- `object['key2'] = 'newvalue2'`

# Operation
- `+ - * / % **(power)`
- `> < >= <=
- `==(is value the same) === (is value AND TYPE the same)`
	- `console.log(5 == '5') // true`
	- `console.log(5 === '5') // false`
- `!=(is value *NOT* the same) !== (is value AND TYPE *NOT* the same)`
	- `console.log(5 != '5') // false`
	- `console.log(5 !== '5') // true`

# Condition
- `if () {}` `else if () {}` `else {}`
- **Terinary Operator** 'short if-else'
	- `(condition) ? ${true; do what} : ${false; do what}`

# Loop
- almost like c 
```JS
let array = [a, b, c, d, e]
for (let i = 0; i < array.length; i++) {
	console.log(array[i]) // a b c d e
}
```
- "for-in" 
 ```JS
 let person = {name: 'John, age: 30, city: "New York"'} 
 for (let key in person) {
	 console.log(key + " = " + person.key)
}
```

```JS
let array = [a, b, c, d, e]
for (let i in array) {
	console.log(array[i]) // a b c d e
}
```
- for-of
```JS
let array = [a, b, c, d, e]
for (let i of array) {
	console.log(i) // a b c d e
}
```
- while
```JS
let array = [a, b, c, d, e]

let i = 0
while (i < array.length) {
	console.log(array[i]) // a b c d e
}
```
- **.map** , **.forEach**
syntax
```JS
[].map((item, index, array) => {})
[].forEach((item, index, array) => {});
```
example
```JS
let array = [a, b, c, d, e]

array.map((item) => {
	console.log(array[i]) // a b c d e
});

array.forEach((item) => {
	console.log(array[i]) // a b c d e
});
```

# Function
syntax
```JS
function myFunc (args) {
}
```
```JS
const myFunc = (args) => {
}
```
how
```JS
function hello() {
	console.log("hello")
}

hello();
```
```JS
const hello = () => {
	console.log("hello")
}

hello();
```