# Method of primitives

## A Primitive
* a value of a primitive value 
* 7 primitives: string, number, bright, boolean, symbol, null, and undefined

## An Object
* capable of storing multiple values as properties
* can be created with {}, or take the form of a function, or other built in objects such as dates, errors, HTML elements etc. which often carries methods

## Properties vs Objects
* objects carry properties and methods; primitives don't
* Objects are "heavier" than primitives

## The Paradox
As we know JavaScript primitives can carry methods
e.g. `'Hello World'.toUpperCase()
` 
For this to work, a **special object wrapper is** is created to wrap the primitive and then destroyed.

1. The string str is a primitive. So in the moment of accessing its property, a special object is created that knows the value of the string, and has useful methods, like toUpperCase().
2. That method runs and returns a new string (shown by alert).
3. The special object is destroyed, leaving the primitive str alone.

This allows primitives to provide methods while remaining lightweight.

<br>
<hr>

## Special Cases:
### Constructors String/ Number/ Boolean are for internal use only
An object is truthy. 

e.g. `new Number(0)` is truthy but `Number(0)` is not, since the later resolves to 0.

String, Boolean, Number are useful for converting value type

### Null have no wrapper objects

