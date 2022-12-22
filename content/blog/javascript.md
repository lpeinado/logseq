---

description: Initial description.

author: "@Luigi"
---

- Here's a nice concise page about Destructuring (different cases)
	- https://www.reactnative.express/javascript/features/destructuring
	- TODO create flashcards for destructuring
	-
- Nullish coalescing operator in Javascript #card
  card-last-interval:: 0.21
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-08-18T14:39:00.192Z
  card-last-reviewed:: 2022-08-18T09:39:00.207Z
  card-last-score:: 3
	- Returns right side if the left side is null or undefined only
	- Will return left side if it is empty string, zero, NaN, etc
		- `console.log(undefined ?? 'ali'); returns ali`
		- `console.log(null ?? 'ali'); returns ali`
		-
- JS primitives
	- Number
	- String
	- Boolean
	- Null
	- Undefined
	- Symbol
- JS objects
	- Array
	- Object
	- Function
- Javascript this
	- This is a keyword NOT variable so you can't change its value
	- this always refers to an Object, depending of how you call it depends which object you refer
		- in an object method, this refers to the object container of the method
		- alone it refers to the global this object
		- in a function, with strict mode, it is undefined
- Javascript strict mode
	- It is implicit in JS modules and classes
	- Converts failures into errors
	- Prevents deleting plane names
	- prevents duplicate property names
	- functions are declared at block level (block level function declaration)