# js-notes: Personal notes about Javascript

```
code
```

## Intro

## Language Basics

### Comments

```javascript
//single line comment
```

```javascript
/* * This is a multi-line comment */
```

### Data Types

Using the typeof operator on a value returns one of the following strings:
* ```"undefined"``` if the value is undefined* ```"boolean"``` if the value is a Boolean* ```"string"``` if the value is a string* ```"number"``` if the value is a number* ```"object"``` if the value is an object (other than a function) or null* ```"function"``` if the value is a function

```javascript
var message = "some string";alert(typeof message);   //"string"
alert(typeof(message));  //"string"
alert(typeof 95);        //"number"
```

### Undefined Type and Null Type

When a variable is declared using var but not initialized, it is assigned the value of undefined as follows:

```javascript
var message;alert(message == undefined); //true
```

Note that a variable containing the value of undefined is different from a variable that hasn’t been defined at all. 

```javascript
var message; //this variable is declared but has a value of undefined
//var age  //age isn’t declaredalert(message); //"undefined"
alert(age); //causes an error
```

The ```typeof``` operator returns ```"undefined"``` when called on an uninitialized variable, but it also returns ```"undefined"``` when called on an undeclared variable.

```javascript
var message; //this variable is declared but has a value of undefined
//var age //age isn’t declaredalert(typeof message);  //"undefined"alert(typeof age);      //"undefined"
```

The Null type is the second data type that has only one value: the special value ```null```. Logically, a ```null``` value is an empty object pointer, which is why ```typeof``` returns ```"object"``` when it’s passed a ```null``` value in the following example:

```javascriptvar car = null;alert(typeof car); //"object"
```

When defining a variable that is meant to later hold an object, it is advisable to initialize the variable to ```null``` as opposed to anything else. That way, you can explicitly check for the value ```null``` to determine if the variable has been filled with an object reference at a later time, such as in this example:

```javascript
if (car != null){	//do something with car}
```Using the equality operator ```(==)``` between ```null``` and ```undefined``` always returns ```true```, though this operator converts its operands for comparison purposes.
Even though ```null``` and ```undefined``` are related, they have very different uses. Never explicitly set the value of a variable to ```undefined```, but the same does not hold true for ```null```. Any time an object is expected but is not available, ```null``` should be used in its place. 

### Global vs Local Variables

Defining a variable inside of a function using var means that the variable is destroyed as soon as the function exits.

```javascript
function test(){	var message = "hi"; //local variable}test();alert(message); //error!
```

Removing the ```var``` operator from the makes the variable global. 

```javascript
function test(){	message = "hi"; //global variable}test();alert(message); //"hi"
```

## Variables, Scope, and Memory

## Reference Types

## Object-Oriented Programming

## Function Expressions

## The Browser Object Model

## JavaScript Design Patterns

## References

* [Derek Sivers: Learning JavaScript - my experience and advice](https://sivers.org/learn-js)
* [Nicholas C. Zakas: Professional JavaScript for Web Developers, 3rd Edition](http://www.wrox.com/WileyCDA/WroxTitle/Professional-JavaScript-for-Web-Developers-3rd-Edition.productCd-1118026691.html)
* [Addy Osmani: Learning JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)
* [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
* [MDN: JavaScript Basics](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/JavaScript_basics)
* [Udacity: Object-Oriented JavaScript	](https://www.udacity.com/course/object-oriented-javascript--ud015)
* [Master the JavaScript Interview: What’s the Difference Between Class & Prototypal Inheritance?](https://medium.com/javascript-scene/master-the-javascript-interview-what-s-the-difference-between-class-prototypal-inheritance-e4cd0a7562e9#.t7st9qu0h)


## Tutorials

* [Beer Drinking Data Vizualization using dc.js, Crossfilter, and Leaflet](https://github.com/austinlyons/dcjs-leaflet-untappd)
* [MDN: 2D Breakout Game using Pure JavaScript](https://developer.mozilla.org/en-US/docs/Games/Workflows/2D_Breakout_game_pure_JavaScript)
* [Build A Real-Time Twitter Stream with Node and React.js](https://scotch.io/tutorials/build-a-real-time-twitter-stream-with-node-and-react-js)
* [anapaulagomes/dashboard](https://github.com/anapaulagomes/dashboard)
* [Master the JavaScript Interview: What is a Closure?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36#.t571z3pw5)

## Tools

* [Leaflet.js](https://github.com/Leaflet/Leaflet)
* [Leaflet.FreeDraw](https://github.com/Wildhoney/Leaflet.FreeDraw)
* [dc.js](https://github.com/dc-js/dc.js)
* [Keshif](https://github.com/adilyalcin/keshif)
* [dc.graph.js](https://github.com/dc-js/dc.graph.js)
* [d3js](http://d3js.org/)