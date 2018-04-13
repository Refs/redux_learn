# redux_learn

## course1 

the first principle of redux -- everything that changes in your application , including the data and the ui stata , is contained in a single object , we call the stata or the stata tree.

## course2 

the second principle of Redux -- the state is read only . the only way to chage the state tree is by dispathing an action. an action is a plain javascript object describing in the minimal way what changed in the application. whether it is initiated by a network request or by user interaction, any data that gets into the redux application gets there by actions 

## course3 

https://www.learnsteps.com/pure-impure-functions/

Difference between pure and impure functions.

* pure functions

These are functions which are sure to provide exact result when the same arguments are passed. For having a function as pure function if must not have any external variable, data store call, ajax request or any other global variables.

This means that you can be completely sure that every time you call the function with the same arguments, you will always get the same result.

```js
function square(x){
     return x*x
}

```
The above function is pure function as we are always certain what will be result and there will be no different results for same input.

* impure functions

When function uses any variables not passed in as arguments, the variables used inside functions may cause side effects. Lets say in case of ajax calls it will fail, In such cases the function is called impure function. When a function depends on variables or functions outside of its lexical scope, you can never be sure that the function will behave the same every time it’s called. Following are impure functions:

```js
function getRandom(number) {
  a = Math.random()
  if(a > 10){
     return a
  }
  else{
     return 10
  }
}

```

Here the function getRandom is impure as it is not sure what will be the result when we call the function.

So this is the difference between pure and impure functions.
