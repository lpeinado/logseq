---

description: Initial description.

author: "@Luigi"
---

- We use the setup() method run before any hook.
- We use reactive from Vue in order to put there the old "data" object and make it reactive.
- We call data as (reactive) state and we put state.whatever in the template
- Don't forget to return (expose) both methods and state in the setup function.
- References to "this" in methods will change to "state" (the reactive one, or whatever name is exported)
- Computed are exported as const with a callback of the computed import
- Hooks are now imported as needed and theres a mapping for them
- setup function is in charge of created and beforeCreate
- hooks are recalled onWhatever except for beforeDestroy and destroyed that now are onUnmounted and onBeforeUnmount
- Props can be accessed directly in the template {{ title }} but in the setup(props) function have to be passed
- watch function has to imported and needs 2 params that are callback functions
	- first param: an arrow function that returns the watched value (usually state.w)
	- sec param: an arrow function with 2 inputs (new, old) and what to do with them.
- using ref
	- you can import ref instead of reactive (refs are reactive)
	- each value is a ref and you get an object, the object returns
		- myThing.value
		- myThing.get()
		- myThing.set()
	- Using ref or reactive depends on the situation is like using a variable or a complex objet with many of them.
	- reactive vs ref: in a reactive composition (reusable) function, if you use reactive instead of ref, then you have to do
		- return toRefs(myThing)
- Composition functions
	- they substitute Mixins
	- they are called with prefix useWhatever
	- they are put in a .js or .ts file so completely out of the framework.
- Teleport
	- used to detach an element for DOM hierarchy to avoid inherit of position fixed or z-index. Usually for modals so you attach the modal content to "body" with teleport.
- Vue2 you had to use this.$set to add/remove properties to be reactive and let Vue detect them
- Vue3 global API methods have mostly changed from Vue.use to app.use
	- app.use
	- app.mount
	- app.directive
	- app app.config.globalProperties
	- app.config.globalProperties.emitter = emitter; emitter = mitt(); (library) to get rid of event bus
	- then with emitter is this.emitter.emit or this.emitter.on("update:goals")
- Suspense
	- For async components (that do a request o the setup function) we can wrap them in a suspense tag with 2 templates: default(the component) and fallback(loading)
	- for the error we decarea a suspenseError ref to null and with the hook called onErrorCaptured we set the ref.value to error.message. So we can wrap the suspense on the v-else of an v-if depending on suspenseError
	- This way we reduce the v-if nesting with loading, success, error and we manage all errors with a single error object (and display the message)
-