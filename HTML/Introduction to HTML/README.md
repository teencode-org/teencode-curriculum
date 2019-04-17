# What is HTML?

HTML (HyperText Markup Language) is a computer language that is used to format websites so that they can be read and displayed in web browsers such as Internet Explorer, Firefox, Safari, Chrome and Opera. You can think of it as a language that is made to tell the web browser how to make a page look.
 
An HTML can be created using a simple text editor (Explain a text editor here).

### Editor:

Since HTML files are just text files, many programs can be used to create them. Some programs provide special assistance for handling HTML, like syntax-highlighting and autocompletion. Example of text editors are notepad, sublime text etc.

## HTML TAGS
### Anatomy of an HTML tag
Each tag has a **"start tag"**, **"end tag"**, some content in between, and optional attributes.

```html
<tagname attribute="value">
  content
</tagname>
```

**Example:**
```html
<a href="http://www.google.com" >
  Google
</a>
```

### What is a Tag
Used by the browser to know how to display content on the screen, also called element

Here is an example of what a tag looks like

```html
<h1>Hello World!</h1>
```
**h1** is an header tag, H stands for Header and 1 is the size

### Putting a Tag Together
A tag is a like a sandwich that made up of a slice of bread , some meat and another slice of bread.

```html
<p> Welcome! </p>
```

<ol>
  <li>**<p> :** This stands for paragraph and it the opening of the p tag (more like the first slice bread in a sandwich)</li>
  <li>**Welcome! :** This is the content which will appear on the browse screen (more like the meat that is put on the first slice bread)</li>
  <li>**</p> :** This is the closing tag for a paragraph it has a forward slash ‘/’ which helps the browser know that it’s the closing tag. (more the the second slice of bread which is used to cover the meat in the sandwich)</li>
</ol>

### What is an Attribute?
Additional values that can adjust the behaviour of the tag. This is like adding butter, Mayonnaise, Egg to our sandwich.

```html
<button id=”SubmitSandwich” class=”btn”> Add Sandwich </button>
```

This button tag as two attributes called id and class.The first attribute is the id attribute. The value of the id attribute can be anything you want it to be,though it can't have any spaces in it. The second attribute is the class attribute. The class attribute can take multiple values, which can be whatever you want them to be. Note: all Attribute are added to the opening tag only.

Global Attribute
<ol>
  <li>id : For Javascript and Cascading style sheets(CSS). No two tag on a page can have the same id value</li>
  <li>class : For Javascript and Cascading style sheets(CSS). Multiple tag can have the same class value on a page.</li>
  <li>style : This is used for inline styling, this should be avoided and only used for testing</li>
  <li>Title : Useds as an identifier or tooltip, when a mouse is hovered over a mouse where the title has being set, then the title is displayed</li>
</ol>

### Elements
<ul>
  <li>Block level element : They take up the whole width of their parent container</li>
  <li>Inline level element : Takes up the current space that it exists in</li>
</ul>
