- Javascript const reserved word is for: #card #javascript
  card-last-interval:: 30.32
  card-repeats:: 4
  card-ease-factor:: 2.66
  card-next-schedule:: 2022-08-24T17:10:37.393Z
  card-last-reviewed:: 2022-07-25T10:10:37.393Z
  card-last-score:: 5
	- Variables assigned that won't reassigned anymore
	- They are not constants as they are still a mutable object (they could be an array that can be "pushed" with new values, but never reassigned with "=" operator)
- Arrow function syntax (many arguments) #card #javascript
  card-last-interval:: 4
  card-repeats:: 2
  card-ease-factor:: 2.32
  card-next-schedule:: 2022-08-13T15:37:21.405Z
  card-last-reviewed:: 2022-08-09T15:37:21.407Z
  card-last-score:: 3
	- If many, arguments they have to be put in parentheses
	  collapsed:: true
		- `x => Math.pow(x, 2)`
		- `(x, y) => Math.pow(x, y)`
		-
		-
		-
- Arrow function 'this' meaning #card #javascript
  card-last-interval:: 19.01
  card-repeats:: 4
  card-ease-factor:: 2.18
  card-next-schedule:: 2022-08-13T10:09:47.790Z
  card-last-reviewed:: 2022-07-25T10:09:47.791Z
  card-last-score:: 3
	- For functions defined with `=>` , the binding for the keyword `this` is the same inside and outside the function.
	- is different than functions declared with `function` , which can bind `this` to another object upon invocation. Maintaining the `this` binding is very convenient for operations like mapping: `this.items.map(x => this.doSomethingWith(x))`
	-
- How arrow functions naming works: #card #javascript
  card-last-interval:: 15.05
  card-repeats:: 4
  card-ease-factor:: 1.94
  card-next-schedule:: 2022-08-09T11:08:02.477Z
  card-last-reviewed:: 2022-07-25T10:08:02.479Z
  card-last-score:: 3
	- Functions defined with `=>` are always anonymous, while functions defined with `function` can optionally be named. Naming can be very helpful in stack traces when debugging, so I recommend using named functions when exporting a function from a file with the `export` keyword.
	- A named function `foo` is defined as `function foo()` , which simultaneously introduces the variable name `foo` into scope. This is different than `const foo = () => {}` , which introduces the variable name `foo` pointing to an anonymous function.
- The `memo` function (react) #card #react
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-09-06T22:00:00.000Z
  card-last-reviewed:: 2022-09-06T14:49:25.198Z
  card-last-score:: 1
	- Is a built in react utility that memorizes the result of a function if with a given input it always returns the same result.
	- Is for improving performance.
	- With memo, a component only re-renders only in case that the input props change.
	- ```
	  import {React, memo} from "react"
	  const CustomContentMemo = memo(CustomContent);
	- ```
	-
- Hooks - useState #card #react
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-10-03T22:00:00.000Z
  card-last-reviewed:: 2022-10-03T11:49:27.916Z
  card-last-score:: 1
	- Is a state related variable that "remembers" its previous value, so it can be updated accordingly (ie counters, adding elements to an array, etc)
	- With a normal variable ( `let a=...`) it will be reset on every component's function call. With useState, React will remember the previous manipulated value and we can increment, modify during the components lifecyle.
	- useState get an argument (initial value) and returns an array with 2 elemnts
		- state, with the current value (initialized)
		- setState, a function to modify the above value within our code.
	- Usage
	  ```
	  import React, { useState } from 'react'
	  const [diceRolls, setDiceRolls] = useState([]) // this initializes to empty array
	  ```
- Hooks - useReducer #card #react
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-10-03T22:00:00.000Z
  card-last-reviewed:: 2022-10-03T11:49:55.314Z
  card-last-score:: 1
	- A similar hook to useState but used with more complex data structures, for instance and object with different keys that we want to modify/update independently from each other. 
	  This is not used in MF codebase
- Hooks - useEffect #card #react
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-10-03T22:00:00.000Z
  card-last-reviewed:: 2022-10-03T11:50:37.441Z
  card-last-score:: 1
	- Is a hook to call a callback function (1st parameter) each time a dependency changes. Dependencies are in an array provided as 2nd parameter.
	  A special usage is done when the dependencies array is empty or undefined:
	  If empty [] the callback function is called only once after the component renders for the 1st time.
	- So this is used to trigger functions when values update or to set values when the component renders.
- Hooks - useRef #card #react
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-09-05T22:00:00.000Z
  card-last-reviewed:: 2022-09-05T14:59:42.015Z
  card-last-score:: 1
	- With `useRef` we can create and update a single mutable value that exists for the lifetime of the component instance. (example: a counter that increments with setInterval, and we can press a button to stop)
	- `const myReference = useRef(initialValue);`
	- After assigning the ref to a variable, we use `.current` to access the mutable value
	- ```
	  import { useRef } from 'react';
	  function MyComponent() {
	    const reference = useRef(initialValue);
	    const someHandler = () => {
	     // Access reference value:
	     const value = reference.current;
	     // Update reference value:
	     reference.current = newValue;
	     };
	   ...
	  - }
	  ```
- Hooks - Custom hooks #card #react
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:36:37.500Z
  card-last-score:: 1
	- They are named as use... for their function names.
	- They are done using the existing built-in hooks.
	- It can be deeply complicated.
	- In (very) brief, a custom hook is a Javascript function with a name that starts with "use" and it calls other reactnative Hooks (useState, useEffect, useRef, use)
- Core components #card #reactnative
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:33:18.184Z
  card-last-score:: 1
	- There are 2 dozens of core components.
		- `import { SafeAreaView, View, FlatList, StyleSheet, Text, StatusBar } from 'react-native';`
	- All of them inherit from the <View> component and all of them accept a style prop
	- Components use the Flexbox algorithm to specify the layout display of their children.
-
- Basic Flexbox #card #flexbox
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-10-03T22:00:00.000Z
  card-last-reviewed:: 2022-10-03T11:51:56.835Z
  card-last-score:: 1
  |  `flexDirection`  |  `column`  |  `row, column`  | Do we want a vertical ( `column` ) or horizontal ( `row` ) layout? This choice determines the orientation of the **primary axis** of our layout. |
  |  `justifyContent`  |  `flex-start`  |  `flex-start, center, flex-end, space-around, space-between`  | How should the content be distributed along the **primary axis** of our layout? Should it be at the start, the center, the end, or spaced evenly? |
  |  `alignItems`  |  `stretch`  |  `flex-start, center, flex-end, stretch, base-line`  | How should the content be aligned along the **secondary axis** of our layout? (If the primary axis is `row` , then the secondary axis is `column` , and vice versa) Should content be aligned at the start, the center, the end, or stretched to fill? |
- Button #card #reactnative
  card-last-interval:: 14.66
  card-repeats:: 4
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-08-09T01:09:42.298Z
  card-last-reviewed:: 2022-07-25T10:09:42.302Z
  card-last-score:: 3
	- Displays a button with the default layout of each platfom.
	- It's convenient but not configurable, so we typically will use a Touchable component instead.
- TouchableOpacity #card #reactnative
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:35:26.893Z
  card-last-score:: 1
	- An area to be pressed and it fades in an out when pressed
	- You can specify an activeOpacity value from 0 to 1 to specify the opacity when pressed.
- Touchables #card #reactnative
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:35:59.347Z
  card-last-score:: 1
	- TouchableOpacity
		- It fades in and out when pressed by default
	- TouchableHighlight (not in MF)
		- Is like the opposite of TouchableOpacity, instead of fading, it hightlights.
	- TouchableWithoutFeedback not recommended by RN documentation
		- Supports only one child. If many child, they have to be wrapped within a View component.
- Lists #reactnative #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.6
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:38:57.327Z
  card-last-score:: 1
	- There are mostly 2 kinds of lists FlatLists and SectionList
- FlatLists #reactnative #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:34:23.763Z
  card-last-score:: 1
	- A component to provide an array of items to be rendered with options, onPress functions, etc.
	- ```
	  return (
	      <SafeAreaView style={styles.container}>
	        <FlatList
	          data={DATA}
	          renderItem={renderItem}
	          keyExtractor={(item) => item.id}
	          extraData={selectedId}
	        />
	      </SafeAreaView>
	    );
	  ```
- Section list #card #reactnative
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.22
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:33:53.231Z
  card-last-score:: 1
	- You can easily build lists within sections (such as the Menu with: Main dishes, sides, drinks)
	- ```
	  const App = () => (
	    <SafeAreaView style={styles.container}>
	      <SectionList
	        sections={DATA}
	        keyExtractor={(item, index) => item + index}
	        renderItem={({ item }) => <Item title={item} />}
	        renderSectionHeader={({ section: { title } }) => (
	          <Text style={styles.header}>{title}</Text>
	        )}
	      />
	    </SafeAreaView>
	  );
	  ```
- Navigation
	- There isn't a "good way" to implement navigation in an app, that's the reason why the library was get off the "react-native" package. There's a "react-navigation" library with many sub libreries:#card #reactnative
		- "react-navigation/core"
		- "react-navigation/stack"
		- "react-navigation/native", "react-navigation/drawers", "react-navigation/bottom-tabs",
	-
	- How navigation commonly works: #card #reactnative
	  card-last-interval:: -1
	  card-repeats:: 1
	  card-ease-factor:: 2.5
	  card-next-schedule:: 2022-08-09T22:00:00.000Z
	  card-last-reviewed:: 2022-08-09T15:37:04.747Z
	  card-last-score:: 1
		- We instantiate a <NavigationContainer /> from library "react-navigation/native"
		- We put in it a Navigation we have created of our choice (stack, bottom-tabs, etc) with
			- <Root.Navigator>...
- AsyncStorage is mostly for #card #reactnative
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.22
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:39:07.559Z
  card-last-score:: 1
	- To store user preferences and client-side persistent data
	- Is a simple key-value store
- AsyncStorage API main methods #reactnative #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:38:34.745Z
  card-last-score:: 1
	- getItem(key:string)
	- setItem(key:string, value:string)
	- removeItem(key)
	- We will usually use JSON.stringify() for the setters and JSON.parse for the getters.
- to run andoid #card
  card-last-interval:: 4.13
  card-repeats:: 2
  card-ease-factor:: 2.46
  card-next-schedule:: 2022-10-04T15:00:57.180Z
  card-last-reviewed:: 2022-09-30T12:00:57.182Z
  card-last-score:: 5
	- yarn android
- to see the list of devices #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-09-07T22:00:00.000Z
  card-last-reviewed:: 2022-09-07T09:24:25.839Z
  card-last-score:: 1
	- adb devices
- React navigation #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-09-30T22:00:00.000Z
  card-last-reviewed:: 2022-09-30T12:00:44.679Z
  card-last-score:: 1
	- React included a native navigation API but they removed it and currently we use the semi-official library called react-navigation
-