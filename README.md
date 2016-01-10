# js-notes: Personal notes about Javascript

```
code
```

##Intro

##Language Basics
###Comments
```javascript
//single line comment
```

```javascript
/* * This is a multi-line * Comment */
```

###Global vs Local Variables

Defining a variable inside of a function using var means that the variable is destroyed as soon as the function exits.

```javascript
function test(){	var message = “hi”; //local variable}test();alert(message); //error!
```

Removing the ```var``` operator from the makes the variable global. 

```javascript
function test(){	message = "hi"; //global variable}test();alert(message); //"hi"
```

##Variables, Scope, and Memory

##Reference Types

##Object-Oriented Programming

##Function Expressions

## The Browser Object Model

##References

* [Derek Sivers: Learning JavaScript - my experience and advice](https://sivers.org/learn-js)
* [Addy Osmani: Learning JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)
* [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
* [MDN: JavaScript Basics](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/JavaScript_basics)


##Tutorials
* [Beer Drinking Data Vizualization using dc.js, Crossfilter, and Leaflet](https://github.com/austinlyons/dcjs-leaflet-untappd)
* [2D Breakout Game using Pure JavaScript](https://developer.mozilla.org/en-US/docs/Games/Workflows/2D_Breakout_game_pure_JavaScript)
* [Build A Real-Time Twitter Stream with Node and React.js](https://scotch.io/tutorials/build-a-real-time-twitter-stream-with-node-and-react-js)
* [anapaulagomes/dashboard](https://github.com/anapaulagomes/dashboard)