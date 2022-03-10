# React Redux

## <ins>Explicitly passing to the store</ins>

- The first, and most logical, way to incorporate the store into your UI is to pass it down the component tree explicitly as a property.

```
const render = () => ReactDOM.render(
  <App store={store}/>,
  document.getElementById('react-container')
)
```

## <ins>Passing the store via context</ins>

- we can take advantage of a React feature called context that allows us to pass variables to components without having to explicitly pass them down through the tree as properties.1 Any child component can access these context variables.

## <ins>Presentation vs Container Components</ins>

- Container components are components that connect presentational components to the data. In our case, container components will retrieve the store via context and man‐ age any interactions with the store.

## <ins>The react redux provider</ins>

- react-redux supplies us with a component that we can use to set up our store in the context, the provider. We can wrap any React element with the provider and that ele‐ ment’s children will have access to the store via context.

```
render(
<Provider store={store}>
<App /> </Provider>,
        document.getElementById('react-container')
    )
```

## <ins>React Redux connect</ins>

- React Redux helps us create container components through mapping the current state of the Redux store to the properties of a presentational component. It also maps the store’s dispatch function to callback properties. This is all accomplished through a higher-order function called connect.
