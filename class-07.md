# Class 07 Reading Notes

Today class we get to learn all about Domain Modeling, HTML Table Basics, Constructors and Object Prototypes.  Frankly, these topics are wildly interesting to me!  More real OOP coding! And the DOM is cool as anything.

## Domain Modeling

### Explain why we need domain modeling

#### From the README.md on Domain Modeling

>Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model. A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

Defining a clean DOM is not easy. I want to understand best practices in more depth.  

This is getting into Constructors but I wanted to include it up front because it is good stuff!

```JavaScript
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```

## HTML Table Basics

### Why should tables not be used for page layouts? (from https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

One shouldn't use tables for layout. Layout tables reduce accessibility. The markup structures are more complex that the screen readers are reading for the visually impaired. The code is also harder to write and maintain. 

In short, using tables for layout rather than CSS layout techniques is a bad idea. The main reasons are as follows:

List and describe 3 different semantic HTML elements used in an HTML `<table>`.

```HTML
<td> //table data
<table> //table element
<tr> //table row
```

## Introducing Constructors

### What is a constructor and what are some advantages to using it?

A constructor is a method that creates an object. It sets up initial values. 

The first version of this is just a function:

```JavaScript
function Person(first, last, age ) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
}
```

### Object Prototypes Using A Constructor

All objects in JavaScript inherit from a `prototype`. They can be chained together. When searching for a member (property or method) first we look at the object we created. If it is not there, then we walk up the chain of prototypes to find it.  Ultimately we reach the end of the object inheritance and get `undefined.`

To find your object's prototype

```JavaScript
Object.getPrototypeOf(myObject);
```

This object has a Date Prototype

```
const myDate = new Date();
let object = myDate;

do {
  object = Object.getPrototypeOf(object);
  console.log(object);
} while (object);
```

Shadowing is when an object in the chain overrides the member(s) in its parent class. 

## Things I want to know more about

Defining a clean DOM is not easy. I want to understand best practices in more depth. ng.
