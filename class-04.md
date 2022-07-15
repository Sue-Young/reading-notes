# Class 04 Reading Notes

This content is important because we are learning about HTML links, JavaScript Functions and CSS Layout.

## HTML Links

We use the anchor tag to create hyperlinks `<a>`. The `href` attribute is the target that contain the web address information.

```HTML
<a href="https://www.mozilla.org/en-US/">the Mozilla homepage</a>.
```

From <https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks>

>A link title is only revealed on mouse hover, which means that people relying on keyboard controls or touchscreens to navigate web pages will have difficulty accessing title information. If a title's information is truly important to the usability of the page, then you should present it in a manner that will be accessible to all users, for example by putting it in the regular text.

## CCS Layout

Normal flow is the way pages lay theselves out if one has not changed their layout specificially.

Static positioning is the default for every HTML element.

### Block-level vs. Inline Elements

Block elements are a kind of blocks where there are many elements in a line itself. While inline elements take up the space of an entire line and there will be only one line within the space width. Inline elements do not respect the top and bottom margins but only the left and right and also consider the padding.

### Absolute Positioning

An absolutely positioned element doesn't exists in the normal document flow.  It is in its own layer which is good for popup boxs, control menus, etc. Also `top`,`bottom`,`left`, `right` are not based off its relative position in the document flow but instead they specify the distance the element should be from the containing element's sides.

### Fixed Positioning vs. Absolute Positionin

The position and dimensions of an element with `position:absolute` are relative to its containing block. The position and dimensions of an element with `position:fixed` are always relative to the initial containing block. This is normally browser window.

## JavaScript

### Function: Declaration and Invocation

A function declaration is where you describe a function: name, list parameters, code block, return, etc.
A function invocation is where you call a function by supplying argument and receiving any return values of interest.
Parameters are described in a function declaration.
Arguments are values passed into a function during invocation.

## Miscellaneous

### Two benefits of Paired Programming

1. Greater efficiency - studies have found that while paired programming may take a little longer when writing the code, the benefits include higher quality code with less defects saving time overall. With someone looking over your shoulder they can double check as you type for bugs. 

2. Engaged collaboration - keeps the coders attention on track. Working with someone keeps both parties paying attention to the development effort. 

## Things I want to know more about

CSS inheritance and overriding.
Using the Google Inspect tools.