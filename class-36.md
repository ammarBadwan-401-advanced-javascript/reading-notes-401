# Application State with Redux

* You can manage the state in redux by combining 3 distinct aspects into a **Store** which all components can access as they please:

1. State.
2. Reducers (strategies to alter state).
3. Actions (Methods that run which trigger reducers).

## Redux Store

* This is where the application's state is stored, it identifies various reducers and middlewares that need to be made available and used globally.

* React uses reducers to hold and manage state, they manage one part of the application state.

* Reducers always hear actions that were dispatched and use the payload they recieved to do their work.

* When an action is dispatched, reducers responds to it and receives that payload and then it does it's actions on the state.

* A **store** is where we declare what middleware you may need and the reducers that you'll use to manage your state data.

* Components subscrite to store and get to use the actions in them.

* Before getting to use the actions, the app needs to have access to the store, the component uses redux's `connect()` method to attach to the store, but first tyou need to provide that to the application or it will fail.

* The `{Provider}` wrapper allows react child components to have access to higher level context.
