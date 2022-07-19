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

### Why should tables not be used for page layouts? (see https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

> In short, using tables for layout rather than CSS layout techniques is a bad idea. The main reasons are as follows:

Layout tables reduce accessibility for visually impaired users: Screenreaders, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screenreaders' output will be confusing to their users.
Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.
Tables are not automatically responsive: When you use proper layout containers (such as `<header>, <section>, <article>, or <div>`), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.

List and describe 3 different semantic HTML elements used in an HTML `<table>`.
from: https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics

> In short, using tables for layout rather than CSS layout techniques is a bad idea. The main reasons are as follows:
> Layout tables reduce accessibility for visually impaired users: Screenreaders, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screenreaders' output will be confusing to their users.
Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.
Tables are not automatically responsive: When you use proper layout containers (such as <header>, <section>, <article>, or <div>), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.


## Introducing Constructors

### What is a constructor and what are some advantages to using it?

How does the term this differ when used in an object literal versus when used in a constructor?

Construtors define the set of methods and the properties it can have — and then create as many objects as we like, just updating the values for the properties that are different.

The first version of this is just a function:

```JavaScript
function createPerson(name) {
  const obj = {};
  obj.name = name;
  obj.introduceSelf = function() {
    console.log(`Hi! I'm ${this.name}.`);
  }
  return obj;
}
```

### Object Prototypes Using A Constructor

Explain prototypes and inheritance via an analogy from your previous work experience.
NOTE: This is a very common front end developer interview question
Bookmark and Review

## Things I want to know more about

Defining a clean DOM is not easy. I want to understand best practices in more depth.  
