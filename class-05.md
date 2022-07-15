# Class 05 Reading Notes

In this class reading we will be covering using images in HTML, using color and styling in CSS.

## HTML Media

### Using Images in HTML

A real world use case to use an `alt` atttribute on and `<img`> tag is to put a description of the image in the alt text so if a visually impaired user is using a screen reader they will have an idea what the image is. 

A real world of using `<figure> <figcaption>` is to link a caption to an image. 

### Common Image Types

Scalable Vector Graphics (SVG)image format is good for user interface elements, icons, diagrams, etc., that must be drawn at different sizes. Graphics Interchange Format (GIF) is good for simple images and animations.

A simple image, like a screenshot of your desktop would be best as a `.gif`. 

## CSS for Using Color

The foreground color usually refers to the text color, and the background color is the color of the background of the element.

To add style an empty blog page, first choose a color scheme that is accessability friendly. Start by choosing a base color and then build out your palette. Keep the color choice small. This is a good tool for building a palette. 

[Paletton](https://www.paletton.com/) 

### Styling HTML text in CSS

There are only a small number of fonts that are generally available across all systems and therefore are good choices for your website fonts. They are aptly called [web safe fonts](https://en.wikipedia.org/wiki/Core_fonts_for_the_Web). 

Since you can't guarantee of the fonts you want even a web font, you can supply a **font stack** so that the browser has multiple fonts it can choose from. This involves a font-family value consisting of multiple font names separated by commas, e.g.,

```CSS
p {
  font-family: "Trebuchet MS", Verdana, sans-serif;
}
```

- `font-size:` sizes the text using many common units
- `font-weight:`sets how bold the font text is
- `font-style:`used to turn italic text on or off

### Two ways to put space around text

1. `letter-spacing` property sets the spacing between letters in your text
2. `word-spacing` property allows you to set spacing between words in your text

## Things I want to know more about

CSS inheritance and overriding.
Using the Google Inspect tools.