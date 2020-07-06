# Context API

* Context provies means of passing statesdown the component tree throught provide/consumer relationship.

* Provide makes it's state available along with means of altering it.

* At lower levels, any component can become a consumer and receive the state from context.

## Class style component

* There are two ways to attach context:

1. Wrap the component with and use a function to get the context object itself.

2. Statically declare a connection to the content provider and use `this.context` to connect a state from the context provider.

## Functional Component

* You can use `useContext()`.

* Returns and provides access to whatever context provider exports.