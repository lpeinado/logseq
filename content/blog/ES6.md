---

description: Initial description.

author: "@Luigi"
---

- [[16th June 2022]] I found this [article](https://dev.to/azure/modern-javascript-10-things-you-should-be-using-starting-today-1adm) . Let's create some flashcards with it
	- Spread operator #card
	  card-last-interval:: 54.59
	  card-repeats:: 5
	  card-ease-factor:: 2.42
	  card-next-schedule:: 2022-10-31T04:48:23.206Z
	  card-last-reviewed:: 2022-09-06T14:48:23.211Z
	  card-last-score:: 3
		- Spread array
		  ```
		  let firstHalf = [ 'one', 'two'];
		  let secondHalf = ['three', 'four', ...firstHalf];
		  ```
		  
		  This is such a nice and compact way of writing it. Doing the same without this would mean doing something like this:NO Array spread
		  ```
		  let firstHalf = [ 'one', 'two'];
		  let secondHalf = ['three', 'four'];
		  for(var i=0, i <firstHalf.length; i++ ) {
		  	secondHalf.push(firstHalf[i]);
		  }
		  ```
	- Rest parameters is: #card
	  card-last-interval:: -1
	  card-repeats:: 1
	  card-ease-factor:: 2.18
	  card-next-schedule:: 2022-09-06T22:00:00.000Z
	  card-last-reviewed:: 2022-09-06T14:47:50.741Z
	  card-last-score:: 1
		- An application of the spread operator to a functions parameters when we don't know how many can be
			- ```
			  function add(first, second, ...remaining){
			  return a + b + remaining.reduce((acc,curr) => acc + curr,0);
			  }
			  ```
			- This functions returns the sum of all the parameters no matter how many we get.
-
- DONE Creating a #css page 
  :LOGBOOK:
  CLOCK: [2022-06-23 Thu 14:29:12]--[2022-06-23 Thu 14:29:17] =>  00:00:05
  :END:
-