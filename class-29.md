# Component Composition

## Routing

* React-router can easily toggle visibility of components (even pages) based on the URL the user engages with using `import {Route} from 'react-router-dom';`.

* To use browser router properly, you use `<Link>` component instead of < a > tags.

* Use the router component to look at a route like `/route` and it displays the route component.

## Component Composition - Logical

* Send the raw data to child component and they render their output as they decide.


## Component Composition - Using Logic-less Children

* It's typically used when a child is already in JSX form and needs you need to display them as a whole, ex: a gallery of images.

## React.js concepts

1. Component Lifecycle: It details the life of a component, it includes:
    1. Mounting.
    2. Updating.
    3. Unmounting.

2. Higher order functions.
3. React state and setState.