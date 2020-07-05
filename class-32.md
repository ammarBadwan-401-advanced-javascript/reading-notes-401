# Custom Hooks

* Custom hooks are duplicated logic from components that share common functionalities (but not state).

* They also take advantage of useEffect lifecycle.


## Common use cases

1. Handle forms easily.
2. Pre-fetch API data.
3. Connect to services (like socket.io).

## Demonstration.

1. Hooks are exported as a function with 'use' prefix.
2. Hooks return data or behaviors that are required to reuse their internal functionality.
3. Hooks are imported in components.
4. Components can re-use the hook as needed.
5. Hooks don't render.

## useReducer hook

* It's alternatice to useState that accepts a state and action and returns the state with a dispatch method.

* Using this is better when you have complex state logic.

* It let's use optimize performance for components that trigger deep updates.

* Example for it: `const [state, dispatch] = useReducer(reducer, initialArg, init);`