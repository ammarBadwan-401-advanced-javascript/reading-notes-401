# Props and State

## Forms and Inputs 

* React form elements maintain internal state.

* The parent component (form container) manages state for all child components of the form and passes state to it's inputs through the use of props.

* Each input has inChange event that handles and updates our form container state.

### Props

* Components accept inputs called props/

* Props is the name of the object passed into a component constructor.

* After passing the props into constructors super function they are available by `this.props`.

* Props can be data or functions, so we can render things using those functions.

### One Way Data Flow

* State can only be passed down the component tree (not up).

* State can only be passed from parent to child component through the use of props.

* If the child wants to pass data to a parent, the parent can pass a function to the child through props and child may invoke that function and pass it data for the parent to manage.

