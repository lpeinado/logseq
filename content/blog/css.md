- To put a value on a css pseudo-element #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 1.94
  card-next-schedule:: 2022-09-05T22:00:00.000Z
  card-last-reviewed:: 2022-09-05T14:58:02.034Z
  card-last-score:: 1
	- Put the content:attr(my-value);
	- ``` .icon-lock:before {
	   content: attr(my-value);
	  ```
	  and
	- ``` 
	  <i class="icon-lock" data-v-17233d1a="" my-value="9"></i>
	  ```
	-
	-
- Now we can translate, scale and rotate in a different way #card
  card-last-interval:: 0.19
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-09-06T18:46:52.912Z
  card-last-reviewed:: 2022-09-06T14:46:52.917Z
  card-last-score:: 3
	- He had to do transform: whatever
	- Now it accepts scale:2, rotate:45deg, and so on
	- This has some nice implications when using them in an animation (it allows to smoothly rotate through values that were set with an css variable and looked chunky)
-