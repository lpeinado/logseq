---

description: Initial description.

author: "@Luigi"
---

- Here we have a page to start working on it #kickstart_reactnative
- React native has some **core components**:
  collapsed:: true
	- <View> is the web equivalent to: #card #reactnative
	  card-last-interval:: 33.96
	  card-repeats:: 5
	  card-ease-factor:: 2.04
	  card-next-schedule:: 2022-10-09T13:56:45.490Z
	  card-last-reviewed:: 2022-09-05T14:56:45.495Z
	  card-last-score:: 5
		- A non-scrollling <div>
	- <Text>  is the web equivalent to: #card #reactnative
	  card-last-interval:: 33.64
	  card-repeats:: 4
	  card-ease-factor:: 2.9
	  card-next-schedule:: 2022-08-28T01:02:48.428Z
	  card-last-reviewed:: 2022-07-25T10:02:48.432Z
	  card-last-score:: 5
		- <p>
	- <Image>  is the web equivalent to: #card #reactnative
	  card-last-interval:: 84.1
	  card-repeats:: 5
	  card-ease-factor:: 2.76
	  card-next-schedule:: 2022-11-29T16:50:13.689Z
	  card-last-reviewed:: 2022-09-06T14:50:13.690Z
	  card-last-score:: 5
		- <img>
	- <ScrollView>  is the web equivalent to: #card #reactnative
	  card-last-interval:: 84.1
	  card-repeats:: 5
	  card-ease-factor:: 2.76
	  card-next-schedule:: 2022-11-29T16:50:22.705Z
	  card-last-reviewed:: 2022-09-06T14:50:22.706Z
	  card-last-score:: 5
		- <div> (scrolling one)
	- <TextInput>  is the web equivalent to: #card #reactnative
	  card-last-interval:: 30.47
	  card-repeats:: 4
	  card-ease-factor:: 2.76
	  card-next-schedule:: 2022-08-24T21:01:16.975Z
	  card-last-reviewed:: 2022-07-25T10:01:16.980Z
	  card-last-score:: 5
		- <input type="text">
	-
- The different types of components can be grouped like this:
  collapsed:: true
	- ![diagram_react-native-components.svg](../assets/diagram_react-native-components_1655207195361_0.svg)
- Currently I'm learning reactnative at #ReactNativeSchool
- React native Build process (theory): #card #reactnative
  card-last-interval:: 15.05
  card-repeats:: 4
  card-ease-factor:: 1.94
  card-next-schedule:: 2022-08-09T11:03:27.595Z
  card-last-reviewed:: 2022-07-25T10:03:27.599Z
  card-last-score:: 3
	- Is used to create standalone binaries of and (Expo) app for iOS and Android which can be submitted to the Apple App Store and Google Play Store.
- Configure App.json for the bundle to be build: #card #reactnative
  card-last-interval:: 15.05
  card-repeats:: 4
  card-ease-factor:: 1.94
  card-next-schedule:: 2022-08-09T11:10:04.531Z
  card-last-reviewed:: 2022-07-25T10:10:04.532Z
  card-last-score:: 3
	- A file that contains the most important parameters for versioning, slug, url, for both iOS and Android
	- ![app dot json.png](../assets/app_dot_json_1656662841699_0.png)
	-
	-
- When installing an npm package globally we use: #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.56
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:35:40.442Z
  card-last-score:: 1
	- npm install --global expo-cli(package)
- To run a global npm command. in MacOS we do: #card
  card-last-interval:: 29.21
  card-repeats:: 5
  card-ease-factor:: 1.94
  card-next-schedule:: 2022-10-04T19:58:57.207Z
  card-last-reviewed:: 2022-09-05T14:58:57.212Z
  card-last-score:: 3
	- npx expo init <projectFolder>
	-
- Once an Expo project is created we can run commands like: #card
  card-last-interval:: 33.32
  card-repeats:: 4
  card-ease-factor:: 2.56
  card-next-schedule:: 2022-08-16T17:04:24.002Z
  card-last-reviewed:: 2022-07-14T10:04:24.004Z
  card-last-score:: 5
	- npm start # you can open iOS, Android, or web from here, or run them directly with the commands below.
	- npm run android
	- npm run ios
	- npm run web
- To make the expo thing work I had to modify the $PATH variable to make the Mac run it, as it wasn't able to find the binaries. Here is how [$PATH explanation](https://stackoverflow.com/questions/62971258/expo-cli-installed-but-when-running-any-expo-command-i-get-zsh-command-not-fou)
- Expo is: #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.08
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:34:57.312Z
  card-last-score:: 1
	- An application that allows you to launch your RN app in web, android or iOS
	- TODO You need an account so the whole thing is stored there.  investigate this more
	-
- A .gitkeep file is: #card
  card-last-interval:: 33.64
  card-repeats:: 4
  card-ease-factor:: 2.9
  card-next-schedule:: 2022-08-28T01:06:52.330Z
  card-last-reviewed:: 2022-07-25T10:06:52.334Z
  card-last-score:: 5
	- https://www.freecodecamp.org/news/what-is-gitkeep/
	- A dummy file to keep track of empty folders. This is because git only keeps track of files, if a folder is empty, it wont add it to the repo, and other developers won't see the folder structure at all.
- To open Development Menu: #card
  card-last-interval:: 28.3
  card-repeats:: 4
  card-ease-factor:: 2.66
  card-next-schedule:: 2022-08-22T17:07:08.127Z
  card-last-reviewed:: 2022-07-25T10:07:08.127Z
  card-last-score:: 3
	- (Cmd+D, Cmd+M, shaking on device)
		-
- To catch up with the rest of the Merryfield team, I have to read [THIS PAGE](https://www.reactnative.express/) notes about it will be taken in page #reactexpress
-
- What are the 2 main rules to remember about Reactnative Hook useRef() #reactnative #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-08-09T22:00:00.000Z
  card-last-reviewed:: 2022-08-09T15:38:08.897Z
  card-last-score:: 1
	- Updating a ref (instantiated via a= useRef()) doesn't trigger the components re-rendering.
	- The value of the ref (myRef.current) persists across the components re-renderings.
- The 3 differences between useRef and useState RN Hooks are: #reactnative #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.22
  card-next-schedule:: 2022-08-18T22:00:00.000Z
  card-last-reviewed:: 2022-08-18T09:51:39.159Z
  card-last-score:: 1
	- Updating ref current value doesn't trigger the component's re-rendering. While updating the state does.
	- Updating the reference is synchronous (updated value is available right away) but updating a state is asynchronous (the new updated value is available after component's re-rendering)
	- Therefore, refs are used mostly for storing infrastructure data of side-effects, while state is mostly for data that has to be rendered or updated in the UI
- One of the most important usages of useRef React Hook is: #reactnative #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-09-05T22:00:00.000Z
  card-last-reviewed:: 2022-09-05T15:02:33.739Z
  card-last-score:: 1
	- Use them to point to a DOM element and then we can access to it for manipulation
	- The way to do it is:
		- Create the ref `const myRefToEl = useRef()`
		- Assign it to the dom element via props: `<div ref="myRefToEl" />``
		- After components rendering, link them: ` useEffect(()=> const divElement = myRefToEl.current = ,[]);
- Dimensions.get('window') vs Dimensions.get('screen') #card #reactnative
  card-last-interval:: 0.21
  card-repeats:: 1
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-09-05T19:55:26.326Z
  card-last-reviewed:: 2022-09-05T14:55:26.332Z
  card-last-score:: 3
  collapsed:: true
	- `window` 's height <  `screen` 's height. So in all likelihood, this means:
	- `window` : reports width/height without the soft menu bar
	- `screen` : reports entire screen's width/height
	- In MF codebase we have many of both