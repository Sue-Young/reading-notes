# Class 09 Reading Notes

We need forms and events to make the web dynamic.

## HTML Forms

### Why are forms important

Forms allow us to ask for input from the user.

### Five form elements

1. `fieldset` groups the form sub elements together
2. `ledgend` gives a title for your fieldset
3. `input` allows you to define an element that allows user data entry of various types
4. `label` allows you to put a text description and it often linked with `input` elements
5. `form` the form keyword itself to encapsulate the other elements

## Events

Events allow for asynchronus actions from the user to trigger actions to happen from the browser into the backend. 

```
addEventListener(type, listener);
```

Takes a `type` which is a case-sentitive string representing the event type to listen for. And a 'listner` which is usually a JS call-back funtion that gets called when the event occurs. 

### The event object

An Event object represents an event which takes place in the DOM. There are lots of different kinds of Events. The target within the event is important because it allows you to access the data entered by the user. 

### Event bubbling vs. capturing 

Event bubbling is when events are sent up from a child element to an ancestor element in the DOM.  Event capturing means the event is sent from the ancestor down to its child elements in the DOM. 

## Things I want to know more about

I love events.  I like forms.  I dislike CSS.  So I need to go back and figure out how to fall in love with CSS.  I need to do the CSS Diner as I have already forgotten the 32 levels of selectors.  I feel like I brute forces some things in CSS already working largely with trail and error.  As an engineer, this does not sit well with me. 