# Class 01 Reading Notes

> This section of reading is important because it describes the basics of how the web works, web design, web process, HTML, Javascript and building web sites.

### HTTP How I Love Thee

> It all began with the DNS,
> giving you my IP address.
> HTTP came riding on TCP/IP,
> asking if my website could come to thee.
> I responded with "200 OK",
> and sent my data packets right away.
> Your browser quickly assembled me
> and our client/server love came to be.

### How HTML, CSS and JS files are Parsed
The browser parses the files in the following order:

- HTML is parsed first recognizing any `<link>` or  `<script>` elements, and sends requests for the CSS or JavaScript files.
- Then parses the CSS and JavaScript.
- In memory DOM tree is generated from the parsed HTML.
- In memory CSSOM from the parsed CSS.
- Compiles and executes the parsed JavaScript.

As the browser builds the DOM, applies the styles from the CSSOM tree and executes the JavaScript, the webpage is rendered to the screen and becomes live to the user.

### Finding Images to add to a Website
Use [Google Images](https://www.google.com/imghp?gws_rd=ssl) and the appropriate Image saving technique for your OS. Google it!

What is not often covered is that most images are copyrighted. Use Google's license filter. Click on the Tools button, then on the Usage rights option. You should choose the option Creative Commons licenses.

### JavaScript String vs. Number Creation
Put simply, Strings are written inside double or single quotes. Numbers are written without quotes.
```
let myString = "This is a String";
let singleQuoteString = 'This is a single quoted string.'
let thisIsAlsoString = "5";
let myNum = 5;
```

### Varibles
Variables are a crutial language construct in all programming languages. A variable is a name/value pair.  The name remains static once declared.  The value can be reassigned during program execution (so long as it is not a Const).

4 Ways to Declare a JavaScript Variable:
Using `var`
Using `let`
Using `const`
Using nothing

### All HTML Elements Can Have Attributes
- Attributes provide additional information about elements
- Attributes are always specified in the start tag
- Attributes usually come in name/value pairs like: name="value"

The <a> tag defines a hyperlink. The href attribute specifies the URL of the page the link goes to:
```
<a href="https://www.restoredyoga.com">Restored Yoga</a>
```

### The Anatomy of an HTML Element
**The Opening Tag:** This consists of the name of the element, wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect.
**The Content:** The content of the element. 
**The Closing Tag:** Same as the opening tag but also includes a forward slash. It marks where the element ends. 
```<p> This is a paragraph tag </p>
```

### Article vs. Section
They are both semantic tags. 

The `<article>` tag contains independant content that doesn't require any other context.
The `<section>` tag is used to split a page into sections like Introduction, Contact, Information, etc. and each section can be in a different `<section>` tag. 

### Elements of a Typical Website

header: `<header>`.
navigation bar: `<nav>`.
main content: `<main>`, with various content subsections represented by `<article>`,`<section>`, and `<div>` elements.
sidebar: `<aside>`; often placed inside `<main>`.
footer: `<footer>`.

### Metadata Influencing SEO
From [Cognitiveseo[](https://cognitiveseo.com/blog/19066/meta-description-affects-seo/#:~:text=In%20short%2C%20Google%20says%20that,backlinks%20tend%20to%20matter%20less.)
> In short, Google says that meta descriptions do not directly impact search engine rankings. However, these descriptions can indirectly impact SEO through click through rates. This is very important when you're fighting between 1st, 2nd and 3rd place. There, things like technical SEO and backlinks tend to matter less.

### How is `<meta>` Used
The `<meta>` tag defines metadata about an HTML document. Metadata is data (information) about data. `<meta>` tags always go inside the <head> element, and are typically used to specify character set, page description, keywords, author of the document, and viewport settings.

### First Step to Designing a Website
Wwhat really matters first is understanding what you want to accomplish. Don't suffer from lack of goals and vision.

Here are a few questions you should answer before anything else:

- What exactly do I want to accomplish?
- How will a website help me reach my goals?
- What needs to be done, and in what order, to reach my goals?

This is called project ideation and is a necessary first step to reach your goal, whether you are a beginner or an experienced developer.

### The Most Important Question
What am I trying to accomplish with this website?  

### Using H1 over Span
In HTML, for example, the `<h1>` element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."
```
<h1>This is a top level heading</h1>
```

By default, most browser's user agent stylesheet will style an `<h1> `with a large font size to make it look like a heading (although you could style it to look like anything you wanted).

On the other hand, you could make any element look like a top level heading. Consider the following:
```
<span style="font-size: 32px; margin: 21px 0;">Is this a top level heading?</span>
```
This will render it to look like a top level heading, but it has no semantic value, so it will not get any extra benefits as described above. It is therefore a good idea to use the right HTML element for the right job.

### Benefits of Using Semantic Tags
Some of the benefits from writing semantic markup are as follows:

-Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
-Screen readers can use it as a signpost to help visually impaired users navigate a page
-Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
-Suggests to the developer the type of data that will be populated
-Semantic naming mirrors proper custom element/component naming

### Two Things that Require JavaScript in the Browser
1. Store useful values inside variables. 
2. Running code in response to certain events occurring on a web page.

### Adding JavaScript to HTML
One way is to use the `<script>` tag inside your HTML.
```
<script>

  // JavaScript goes here

</script>
```
You can also include an external JavaScript file. 
```
<script src="script.js" defer></script>
```

You can also have JavaScript code inside the HTML.
```
function createParagraph() {
  const para = document.createElement('p');
  para.textContent = 'You clicked the button!';
  document.body.appendChild(para);
}
```
```
<button onclick="createParagraph()">Click me!</button>
```