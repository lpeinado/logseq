---

description: Initial description.

author: "@Luigi"
---

- UNIT TESTING
	- There are 2 kinds of unit tests #card #vue
		- Whitebox (unit testing)
		  Blackbox (component testing)
	- Whitebox tests #card #vue
		- Take care of the implementation details and they usually need to mock some children components or state values
	- Blackbox tests #card #vue
		- They don't take care of the details and mock as less as possible. They are kinda integration tests and will usually render all child components.
	- Technologies on Vue testing #card #vue
		- Vitest, is the recommended bc create-vue is based on Vite
		- Peeky created by Vue core team members and nice Vite integration
		- Jest only recommended if legacy. Using vite-jest package.
	- Vue component tests #card #vue
		- They are considered Integration test and interact with the component as the user should instead of taking care of the details. They are above unit testing.
		- They can be done with library @testing-library/vue
- COMPOSITION API
	- What are composables #vue #card
		- They are functions that leverage Composition API in order to encapsulate and make reusable stateful logic.
		- They are equivalent to React custom hooks: they must be named as useWhatever and can also use other hooks (onMounted, onUnmounted)
	- What is stateful and stateless logic #vue #card
		- stateless: a time format function that retrieves and output given an input value
		- stateful: the result depends on the state values, like a connection status to a database.
		  reta.barcelona@activamutua.es con tramitacion.
	- VUE ESlint recommended rules to let many rood tag nodes in a template #card
		- You have to change the eslintrc rule instead of using vue/recommended -> vue/vue3-recommended