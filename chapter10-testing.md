# Testing

## <ins> eslint </ins>

- linters provide hints to enforce code style guidelines

## <ins> testing redux </ins>

- Testing is essential for Redux because it only works with data—it does not have a UI. Redux is naturally testable because its reducers are pure functions

#### test driven development

- Process where tests are written first before code

#### testing reducers

- Reducers are pure functions that calculate and return results based upon the input arguments.
- the packaage deepfreeze can be used to unsure that objects arent changing and maintaining a functional approach

#### testing the store

- While testing the store you can integrate your action creators and kill two birds with one stone, testing the store and the action creators together.

## <ins> testing react components </ins>

#### setting up jest enviornment

- Jest provides us with the ability to run a script before any tests are run where we can set up additional global variables that can be used in any of our tests.

package.json

```
   "jest": {
      "setupFiles": ["./__tests__/global.js"],
      "modulePathIgnorePatterns": ["global.js"]
}
```

#### enzyme

- Enzyme makes it easier to render a component and traverse the rendered output.

#### mocking components

- Mocking allows you to isolate, build, and test functionality independently of other components.
- One place where we will need to use mocks is when we are testing higher-order com‐ ponents.

## <ins> snapshot testing </ins>

- Snapshot testing provides us with a way to quickly test UI components to make sure that we have not caused any unexpected changes

## <ins> using code coverage </ins>

- Code coverage is the process of reporting on how many lines of code have actually been tested.
