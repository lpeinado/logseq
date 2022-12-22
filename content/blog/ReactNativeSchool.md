---

description: Initial description.

author: "@Luigi"
---

- My courses can be found here [Courses Dashboard](https://learn.reactnativeschool.com/courses/enrolled)
- # React Native Basics: Build a Currency Converter
	- We are gonna use Expo, that allows you to get RN working with a simple npm package.
	  collapsed:: true
		- Expo is a superset on RN, you can always use RN CLI but the course is going to be on Expo.
		- [[16th June 2022]] https://learn.reactnativeschool.com/courses/175915/lectures/17441005
		- We install expo with: #card
		  card-last-interval:: 16.65
		  card-repeats:: 4
		  card-ease-factor:: 2.04
		  card-next-schedule:: 2022-08-11T01:08:12.699Z
		  card-last-reviewed:: 2022-07-25T10:08:12.706Z
		  card-last-score:: 3
			- npm install expo-cli --global (we need node.js already installed)
		- During the Module 3 I learned some basics and components
			- Components that I use to build UI on react native #reactnative #card
			  card-last-interval:: 22.92
			  card-repeats:: 4
			  card-ease-factor:: 2.32
			  card-next-schedule:: 2022-08-17T08:11:52.227Z
			  card-last-reviewed:: 2022-07-25T10:11:52.229Z
			  card-last-score:: 3
				- ```
				  import {View, Text, TouchableOpacity, StyleSheet}
				  ```
		- To create styles in a react native components #reactnative #card
		  card-last-interval:: 15.05
		  card-repeats:: 4
		  card-ease-factor:: 1.94
		  card-next-schedule:: 2022-08-09T11:07:52.683Z
		  card-last-reviewed:: 2022-07-25T10:07:52.687Z
		  card-last-score:: 3
			- ```
			  import {StyleSheet} from "react-native"
			  and then
			  const styles = StyleSheet.create({
			          name:{}, name2:{}
			  }
			  );
			  ```
			- A custom component accepts props when created such as #card
			  card-last-interval:: 4
			  card-repeats:: 2
			  card-ease-factor:: 1.94
			  card-next-schedule:: 2022-09-09T14:55:50.905Z
			  card-last-reviewed:: 2022-09-05T14:55:50.906Z
			  card-last-score:: 3
				- ```exportconstRowItem  = ({text, rightIcon, onPress }) => {
				  return(
				  <TouchableOpacity style={styles.row} onPress={onPress}>
				    <Text style={styles.text}>{text}</Text>
				    {rightIcon}
				  </TouchableOpacity>);
				   };
				   
				  ```
- The way to make an area scrollable is to use: #card
  card-last-interval:: 26.66
  card-repeats:: 4
  card-ease-factor:: 2.56
  card-next-schedule:: 2022-08-21T01:02:56.912Z
  card-last-reviewed:: 2022-07-25T10:02:56.917Z
  card-last-score:: 5
	- ```
	  <ScrollView />
	  ``` 
	  and put all the content within
- The way to make an area get all the room available is to set:
	- ```
	  <SafeAreaView style={{flex:1}}> ...
	  ```
- To open links with the app we may use: #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.22
  card-next-schedule:: 2022-09-07T22:00:00.000Z
  card-last-reviewed:: 2022-09-07T09:18:11.493Z
  card-last-score:: 1
	- ```
	  import { Linking} from "react-native";
	  const link = (url) =>{
	     return Linking.openURL(url).catch(Alert.alert("something failed"))
	  }
	  ```
	-
- Regarding Images I've learned: #card #reactnative
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.22
  card-next-schedule:: 2022-09-07T22:00:00.000Z
  card-last-reviewed:: 2022-09-07T09:15:34.742Z
  card-last-score:: 1
	- import Image and Dimensions
		- `import {Image, Dimensions} from "react-native"`
	- Image has properties of style, source (with a require), and resizeMode (contains, etc)
	- resizeMode is set by default to "cover", but it can be: cover, contain, stretch, repeat, center.
	- ```
	  <Image 
	            style={styles.logo} 
	            source={require("../assets/images/logo.png")} 
	            resizeMode="contain"
	    />
	  ```
- Regarding Dimensions function we have to remember: #card #reactnative
  card-last-interval:: 4
  card-repeats:: 2
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-08-22T09:48:47.381Z
  card-last-reviewed:: 2022-08-18T09:48:47.390Z
  card-last-score:: 3
	- We import it from react-native
	- We use it like:
	  ```
	  const screen = Dimensions.get("window")
	  ...
	  logo: {
	      position: "absolute",
	      width: screen.width * 0.25,
	      height: screen.width * 0.25,
	     
	  ```
	- At MF we can see it usage like:
	  ` const { height: windowHeight, width: windowWidth } = Dimensions.get('screen'); `
	- This is imported from react-native library.
- A new empty component in Reactnative can be created with: #card #reactnative
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:34:44.795Z
  card-last-score:: 1
	- ```
	  export const ConversionInput = () => null;
	  ```