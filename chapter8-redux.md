# Redux

- designed to tackle the challenge of under‐ standing how data changes flow through your application

## state

- Redux simplifies the way we view state in our application by requiring us to store all state data in a single object. Everything we need to know about the application is in one place: a single source of truth

## actions

- We will eventually update this state object by replacing it entirely. In order to do this, we will need instructions about what changes. That’s what actions provide: instructions about what should change in the application state along with the neces‐ sary data to make those changes.

#### action payload data

- Actions are JavaScript literals that provide the instructions necessary to make a state change.

```
{
   type: "ADD_COLOR",
   color: "#FFFFFF",
   title: "Bright White",
   rating: 0,
   id: "b5685c39-3bdc-4727-9188-6c9a33df7f52",
   timestamp: "Sat Mar 12 2016 16:12:09 GMT-0800 (PST)"
}
```

## reducers

- Reducers are functions that take the current state along with an action as arguments and use them to create and return a new state.

#### the color reducer

- handles updating of specific color objects

#### the colors reducer

- the color reducers can be composed toupdate the entire color array

## the store

- the store is what holds the application’s state data and handles all state updates

#### subscribing to stores

- Stores allow you to subscribe handler functions that are invoked every time the store completes dispatching an action

## action creators

- Action objects are simply JavaScript literals. Action creators are functions that create and return these literals.
