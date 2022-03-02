# React with JSX

- <ins>prop types</ins> : used to type check props
  - can also be used to ensure that a value was supplied

```
propTypes: {
ingredients: PropTypes.number.isRequired, steps: PropTypes.number.isRequired, title: PropTypes.string
},
```

- <ins>default props</ins> : used when a prop is not input

```
  getDefaultProps() {
        return {
            ingredients: 0,
            steps: 0,
            title: "[recipe]"
}
```

- <ins>custom prop validation</ins> : Allows you to test the properties in many different ways

```
propTypes: {
ingredients: PropTypes.number, steps: PropTypes.number, title: (props, propName) =>
}
(typeof props[propName] !== 'string') ?
  new Error("A title must be a string") :
  (props[propName].length > 20) ?
      new Error(`title is over 20 characters`) :
      null
```

- <ins>refs</ins> : used to modify child components outside of the normal data flow

- <ins>two way data binding</ins> : sending a callback function to the component as a property that the component can use to pass data back as arguments

- <ins>state</ins> : states values update the UI when state changes. The UI is a representation of the state of the application
