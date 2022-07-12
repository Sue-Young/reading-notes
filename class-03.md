# Class 03 Reading Notes

This content is important because it will be teaching us about HTML Lists, Control Flow with JS, and the CSS Box Model!

## HTML

### Ordered and Unordered lists

The `<ul>` is for grouping a collection of items that do not have a number ordering, and their order in the list is random.

Use the Attribute `type` to set the bullet style.

- `circle`
- `disc`
- `square`

Unordered list is used to create a list of related items, in no particular order. Ordered list is used to create a list of related items, in a specific order.

You can change the `list items` on an `ordered list` using the `type` attribute.

type="1" The list items will be numbered with numbers (default)
type="A" The list items will be numbered with uppercase letters
type="a" The list items will be numbered with lowercase letters
type="I" The list items will be numbered with uppercase roman numbers
type="i" The list items will be numbered with lowercase roman numbers

```HTML
<ol type="A">
  <li>List</li>
  <li>Using</li>
  <li>Uppercase Letters</li>
</ol>
```

## CSS

### The Box Model Story

Once upon a time there was an image that want to lay out nicely on a webpage. First the image needed to get a little space from its border. The border was too close. So the image asked her friend padding to come and wrap around her like a blanket, giving her some space from border.  This made her happy inside. But getting a little space from her border was not enough. As soon as she laid down in her webpage she noticed she was much to closer to the other images already asleep on her page. So next she invited her friend padding to tea. She asked padding if he could grow a little and put more space between her and the other images.  He did and everything was jusssst right.

### Four parts of an HTML box model

- **Content box:** the area where  content is displayed
- **Padding box:** the padding around the content as white space
- **Border box:** the border box wraps the content and any padding
- **Margin box:** the margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements

## Javascript

### Arrays

You can store strings, numbers, objects, and other arrays within an array - called a multidimensional array.

```JavaScript
const shopping = ['bread', 'milk', 'cheese', 'hummus', 'noodles'];
shopping[0] = 'tahini';
console.log(shopping);
// shopping will now return [ "tahini", "milk", "cheese", "hummus", "noodles" ]

const random = ['tree', 795, [0, 1, 2]];
random[2][2];
```

Is this valid syntax?

```Javascript
const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
```

Yes. This is a multidimensional array. You access this array with double bracket notation.

```Javascript
// to return 'pete'
people[0][0];
```

### Operators

#### Five shorthand assignment operators

- Addition assignment x += f(), adds the value of f() to x and then assigns it to x.
- Subtraction assignment x -= f(), subtracts the value of f() from x and then assigns it to x.
- Multiplication assignment x *= f() multiplies the value of f() times x and then assigns it to x.
- Division assignment x /= f() divides x by f() and then assigns it to x.
- Remainder assignment x %= f() divides x by f() and assigns the remainder to x.

#### Evaluting Expressions

This bizzare piece of code has Javascript "adding" a number, a string and a boolean.

```Javascript
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
 ```

The `+` operator here promotes `a` into a String datatype and concats it with `b`. The result is
`10dog`. I guess the boolean can't be coerced into anything so is just ignored? Question for class.

#### Conditionals

Conditionals execute a set of code if a condition is true. A real world example might be to throw an alert if a user does not enter a valid form of data. This is error handling.

#### Loops

Loops are useful when you need to iterate over a set of data while a condition is true. So perhaps you want to keep asking the user to enter data until they type "STOP". A while loop will allow you to continue to prompt until the user signals they are done.

## Things I want to know more about

The topics of block and inline boxes, outer display type, inner display type, etc. frighten me. I guess this means I want to know more about them?
