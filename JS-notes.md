# JavaScript Reading Notes

JavaScript (JS) is a compiled programming language with functions. It is most well-known as the scripting language for Web pages.

[JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide) is a deatailed guide to the JS language.

JavaScript [Complete Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)

## The script tag in HTML

Here is an example of some JS in an HTML file

```
<script>
function say_hi() {
    var fname = document.getElementById('first_name').value;
    var lname = document.getElementById('last_name').value;
 
    var html = 'Hello <b>' + fname + '</b> ' + lname;
 
    document.getElementById('result').innerHTML = html;
}
```
Look at how easy this!  Amazingly cool. It has functions and variables, oh my! Actual real coding. 