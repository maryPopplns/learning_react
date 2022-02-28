# Functional Programming

- <ins>first class functions</ins> :(functions can do the same things variables can do)
- <ins>imperative programming</ins> : style of code that is only concerned how to achieve results with code

```
var string = "This is the midday show with Cheryl Waters";
var urlFriendly = "";
for (var i=0; i<string.length; i++) {
  if (string[i] === " ") {
    urlFriendly += "-"; }
  else {
    urlFriendly += string[i];
  }
}
```

- <ins>declarative programming</ins>: prioritizes describing what should happen, not how it should happen

```
const string = "This is the mid day show with Cheryl Waters"
const urlFriendly = string.replace(/ /g, "-")
```

## Functional Concepts

- <ins>immutability</ins>: sdata cannot be changed
- <ins>pure function</ins> : a function that returns a value that is computed based on its arguments, they do not cause side effects, set global variables, or change anything about application state.
  - Pure functions are naturally testable. They do not change anything about their environment or “world,” and therefore do not require a complicated test setup or teardown
- Pure functions should be:

  1. The function should take in at least one argument.
  2. The function should return a value or another function.
  3. The function should not change or mutate any of its arguments.

- <ins>Higher-order functions</ins> : functions that can manipulate other functions. They can take functions in as arguments, or return functions, or both.
- <ins>Recursion</ins> : functions that can call themselves
- <ins>Composition</ins> : Functional programs break up their logic into small pure functions that are focused on specific tasks. Eventually, you will need to put these smaller functions together. Specifically, you may need to combine them, call them in series or parallel, or compose them into larger functions until you eventually have an application.
  - The goal of composition is to “generate a higher order function by combining simpler functions.”
