# Enhancing Components

## <ins> Component Lifecycles <ins/>

- methods that are invoked in series when a com‐ ponent is mounted or updated

#### Mounting lifecycle

- methods that are invoked when a component is mounted or unmounted

#### Updating lifecycle

- series of methods that are invoked when a component’s state changes or when new properties are received from the parent

#### React Children

- provides a way of working with the children of a particular component
  - allows you to count, map, loopover, or convert props.children to an array
  - allows you to verify that you are displaying a single child with React.Children.only

## <ins> Higher Order Components </ins>

- a function that takes a React component as an argument and returns another React component
- great way to reuse functionality and abstract away the details of how component state or lifecycle are managed

## <ins> Managing state outside of react </ins>

## <ins> Flux </ins>

- is a design pattern developed at Facebook that was designed to keep data flowing in one direction

#### Actions and Action Creators

- Actions provide the instructions and data that the store will use to modify the state

#### Dispatcher

- The dispatcher takes the action, packages it with some information about where the action was generated, and sends it on to the appropriate store or stores that will handle the action.

#### Stores

- Stores are objects that hold the application’s logic and state data
