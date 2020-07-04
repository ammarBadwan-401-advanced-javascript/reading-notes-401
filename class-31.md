# Hooks API

## Hooks

* React hooks allow to easily create and manage state in a functional component.

* Hooks additional rules:

1. Must start with 'use' like `useCar`.
2. Only call them at top level, not inside loops, conditions or nested functions.
3. Call hooks from react function components only.

## Built in Hook

* It returns a stateVariable and setter function to manage state in a functional component.

* By convention, use set and the variable name you want, for example variable is car, we use `setCar`.

* Then, useing `useState()` that takes a single param which is the value you want to assign the state variable to.

* You can call you set function and the value in the same sentence,for example `setCar('driving')`.

* Example: 

`const [car,setCar] = useState('driving')`