# <Login /> and <Auth />

## Authentication + Role Based Authorization

* We need to solve problems for:

1. Is this a valid user.
2. What are they authorized to do.
  - Which part of the app cares about this
  - We need token to determine this.


## Proposal

`<Auth />` component.

* Based on the permission and login status, it either gives you access to a component or jsx or hides it.

* Must not use Redux because we don't want to force implementation into a specific state management system.

* This is an example for Auth 

## React Cookies

Install it with `npm i react-cookies`

* Then import it and save it as a state by `cookie.load('token')`

```Javascript
// The div only shows if you are logged in
  <Auth>
    <div />
  </Auth>

  // The div only shows if you are logged in AND have read permissions
  <Auth capability="read">
    <div />
  </Auth>
```