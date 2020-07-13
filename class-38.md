# Redux - Asynchronous Actions

## Thunking for Data

* Using redux actions to connect to remote API's via Thunk Middleware.

* Normally, action generators return a function but often you will need your actions to do some async actions before you disspatch it to the reducer.

* In this case we want to set it up like this, where the action you dispatch from react app returns a function and not an actual action object, which is what redux expects and requires.

* To do that, we need to use a special redux middleware called **thunk** which inspects every dispatched action and either lets it go through or it processes the function and dispatches what that function returns.

* The function recieves a `dispatch()` which it calls with the payload it got from the server.


* In redux, middlewares are implemented as curried function that evaluate the action, if so it gets invoked with dispatch and getstate methods otherwise it simply runs the action.
