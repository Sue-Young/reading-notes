# Class 06 Reading Notes

This reading note is all about JavaScript Objects and the DOM. 

## JavaScript Objects

An object is a package of data and behavior.  Lets say we have a dog and we want to model it in a JavaScript object.  You dog has a name and 4 legs (data).  It loves to run and bark (behavior). In JavaScript your dog would look like this:

```JavaScript
const dog = {
  name: 'Fido',
  legCount: 4,
  run: function (){
    console.log(`${this.name} loves to run!`);
  },
  bark: function (){
    console.log(`${this.name} loves to bark!`);
  }
}
```

Object litererals are a nice way to package up data beyond an array.  For example, sending a package of data over the net to a database. They are more efficent than sending individual pieces of data.

It can be helpful to think of objects as associative arrays.  Object declare a namespace and map strings to values in the same way that arrays map numbers to values.

Usually we access an object with the dot notation. 

```JavaScript
const person = {
  name : {
  first: 'Bob',
  last: 'Smith'
  },
  age: 32,

  bio() {
    console.log(`${this.name[0]} ${this.name[1]} is ${this.age} years old.`);
  },
  introduceSelf() {
    console.log(`Hi! I'm ${this.name[0]}.`);
  }
};

person.name.first
person.name.last
```

We can also access an objects properties using `[]` bracket notation. This is necessary if an object property name is defined at runtime.

```JavaScript
person['age']
person['name']['first']
```

Example of defined at runtime.

```JavaScript
const person = {
  name: ['Bob', 'Smith'],
  age: 32
}
const input = prompt('Get name or age?')
console.log(person[input])
```

In this piece of code defines an object named dog with 4 **members** (name/value pair): 3 **properties** and 1 **method**. The object's name `dog` acts as a namespace. The `this` notation allows you to access the other members of this object. 

```JavaScript
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

## The Document Ojbect Model (DOM)

The DOM represent a webpage so we can programmatically change the document structure, style and content. The DOM represents the document as nodes and objects. This allows languages like JavaScript to manipulate it. All of the properties, methods, and events available for manipulating and creating web pages are organized into objects.

Code is written in JavaScript and JavaScript **uses** the DOM to access the document and its elements. 

```JavaScript
const paragraphs = document.querySelectorAll("p");
// paragraphs[0] is the first <p> element
// paragraphs[1] is the second <p> element, etc.
alert(paragraphs[0].nodeName);
```

## Things I want to know more about

CSS inheritance and overriding.
Using the Google Inspect tools.