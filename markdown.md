## What is Markdown?

> Markdown is actually a simple Markup syntax

Confusing, right? Why John Gruber and Aaron Swartz, the creators of Markdown, decided to go with Markdown instead of MarkupLite, is unfortunate. 

Regardless of the misnomer, Markdown serves an important role in the Markup world. It is a text Markup that is designed for readability. Unlike HTML, Markdown has no tags. You can read and write Markdown with simple plain text annotations. This is useful in technical documentation and has been adopted by open source heavy hitters like Git/GitHub. 	

GitHub has a wonderful [Markdown Syntax Guide](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax). 

To decide for yourself if Markdown is more human readable than HTML tag syntax, here is a sample of just a few things you can do with Markdown.  

```markdown

The first and most important devleoper Markdown is the comment.  

<!-- Good for commenting your Markdown AND blocking out Markdown that you don't want rendered. -->


Perhaps the least important developer Markdown is the emoji. But let's live a little. 

Alice in :chains:


Markdown is useful for Styling Text:

1. **Two asterisks make it Bold**  
2. _One underscore is Italic_  
3. ***Three asterisks are both Bold and Italic***



To get Headers 1-6 use Hash Signs:

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6


You can easily produce Ordered and Unordered Lists:

- Unordered list element 1
- Unordered list element 2

1. Ordered list element 1
2. Ordered list element 2


Links and Images too. The fun stuff:

[Link](url) and ![Image](src)
```


One last note, Markdown is converted into HTML by a static site generator. So all those lovely tags are still there, they are just created for you. Woo hoo!

