# Class 02 Reading Notes

This content is important as it furthers our understanding of HTML, CSS and JavaScript. 

## Introduction to HTML

### Semantic Elements in HTML

The most important reasons to use semantic markup are:

1. Clearer code and therefore easier to maintain
2. Help your site be accessible
3. Improve SEO

### Header Levels

HTML defines six levels of headers.

### Uses for `<sup>` and `<sub>` Elements

The `<sup>` tag defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes.

The `<sub>` tag defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas

### The `<abbr>` Element

Use the global `title` attribute to show the full expansion for the abbreviation when you mouse over the element.

## Onto CSS

### Ways to Apply CSS

1. external stylesheet
2. internal stylesheet
3. inline styles

### Inline Styles are Not Best Practice

1. least efficient implementation of CSS for maintenance, could require multiple edits
2. mixes CSS presentation code with HTML and content, hard to read and understand

You want to separate code and content.

### Code Review

1. What is representing the selector?
h2
2. Which components are the CSS declarations?
    color: black;
    padding: 5px;
3. Which components are considered properties?
    color:  
    padding:  

## JavaScript

A String is defined by single quotes.

```JavaScript
let myVariable = 'Code Fellows';
```

### Four Types of JavaScript Operators

1. Arithmetic
2. Comparison
3. Assignment
4. Logical

### Real World Usage of Function

Create a function that concats two strings.  Pass in two strings and return a joined string.

### Conditionals

An if statement checks a condition and if it evaluates to true then the code block will execute.

An `else if` statement will execute when the first `if` is false but the second `if` is true.

### Comparison Operators

1. `==` equal to
2. `===` equal value and equal type
3. `!=` not equal

Logical `&&` and. Both conditions must to true to evaluate to true.
Logical `||` or. Only one condition must be true to evaluate to true.

## Things I want to know more about

CSS inheritance and overriding.
Using the Google Inspect tools.
