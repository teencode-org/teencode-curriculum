# HTML Tags and Structure

```html
<span></span>
```
<ul>
  <li>This is a inline element</li>
  <li>Used for grouping text together that you want to keep inline</li>
  <li>Attributes : Global</li>
</ul>


```html
<p></p>
```

<ul>
  <li>Represent a paragraph of text</li>
  <li>Block Level</li>
  <li>Used for display lot of text</li>
  <li>Allow only Global Attributes</li>
</ul>


```html
<div></div>
```

<ul>
  <li>div stands for division</li>
  <li>Block Level</li>
  <li>This is used as a block container and also used to group together other tags</li>
</ul>


```html
<sub></sub>
```

<ul>
  <li>sub stands for Subscript</li>
  <li>Inline element</li>
  <li>This is used when we need text to appear lower that other text</li>
  <li>E.g h20</li>
</ul>


```html
<sup></sup>
```

<ul>
  <li>sup stands for Superscript</li>
  <li>Inline level</li>
  <li>This is used to show text that need to appear over other text</li>
  <li>E.g E = mc2</li>
</ul>

```html
<u></u>
```

<ul>
  <li>Underline a span of text</li>
  <li>Inline level</li>
  <li>Used to underline certain text</li>
</ul>

```html
<em></em>
```

<ul>
  <li>Emphasize span of text</li>
  <li>Inline</li>
  <li>Used to emphasize certain text which appears italicized</li>
</ul>


```html
<strong></strong>
```

<ul>
  <li></li>
</ul>

```html
<br>
```

<ul>
  <li>Breaks text</li>
</ul>

```html
<ul></ul>
```

<ul>
  <li>Used to create an unordered list</li>
</ul>


```html
<ol></ol>
```

<ul>
  <li>Used to create a ordered list</li>
</ul>


```html
<img src="smiley.gif" alt="Smiley face" /> 
```

<ul>
  <li>Used to define an image in html</li>
  <li>It has 2 required attributes: src and alt</li>
  <li>src specifies the URL of the image</li>
  <li>alt specifies an alternate text for the image</li>
</ul>

```html
<a href=”https://wwww.google.com” />Go to google</a>
```

<ul>
  <li>Defines an hyperlink, which is used to link from one page to another</li>
  <li>The href tag is important, as it indicates the link’s destination.</li>
</ul>

### Ordered and Unordered lists.
An unordered list starts with the **<ul>** tag. A ordered list starts with the **<ol>** tag Each list item starts with the **<li>** tag.

*Example of unordered list:*
The list items will be marked with bullets by default.
```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

**Result**

```
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

*Example of ordered list:*
The list items will be marked with numbers by default:

```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

**Result**
```
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```