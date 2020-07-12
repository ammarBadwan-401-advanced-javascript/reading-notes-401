# Redux - Combined Reducers

## Combined Reducers

* Combined reducers are nothing more than pulling in more than one reducer and creating a keyed object from them.

* Once its done, all components can reach into the store and get any of the reducers.

## Why?

* To Obey the single responsibility principle
    * Reducers really should have only 1 part of state to manage.
    * It's more work/boilerplate.
    * It allows for logic decoupling.

## Actions

* Each reducer has it's own actions and creators.

* Reducers can crossover and both be dispatched.

* If an action is dispatched with both reducers recieving it, both would respond to it.

* It's very powerful but it needs to be understood well or it will cause unforseen consequences.