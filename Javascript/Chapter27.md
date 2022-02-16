# Chapter 27 Async JavaScript

## The Call Stack
It is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions
- Last thing in, First thing out

## WebAPIs & Single Threaded
### Single Threaded
Non-blocking. It has only one call stack. Whatever is on the top of the call stack is run first.<br>
(WebAPI might need some time to be loaded)

## Call back hell 
It is an anti-pattern seen in code of asynchronous programming. It is a slang term used to describe and unwieldy number of nested 'if' statements or functions.

## Promises
A promise is an object representing the eventual completion or failure of an asynchronous operation

## Async functions
A newer and cleaner syntax for working with async code. Syntax 'makeup' for promises
- Async
- Await

### The async keyword
- Async functions always return a promise
- If the function returns a value, the promise will be resolved with that calue
- If the function throws an exception, the promise will be rejected

### The await keyword
- We can only use the await keyword inside of functions declared with async.
- await will pause the execution of the function, waiting for a promise to be resolved

## Handling Errors in Async Functions
`try` and `catch`

 
