# HTML Basics
The doctype isn't an actual tag, but it needs to be at start at every HTML page to tell browser which version of HTML you're using (HTML5, in example below).

The html tag is always the first tag in the page, everything goes

```html
<!DOCTYPE html>
<html>
</html>
```

### Head & Body
The head contains **"meta"** information about the page, information that the browser needs before rendering it.

The body contains the actual content of the page.

```html
<!DOCTYPE html>
<html>   
 	<head>
		<meta charset="utf-8">
		<title>Title of your page goes here</title>
	</head>
 	<body>
		Bulk of your content here.
	</body>
</html>
```

### What Goes in the body
Headlines, Paragraphs, Line breaks, Lists, tags etc.

### Room for Improvement
<ul>
  <li>Mention best practices for HTML style - using quotes, pressing enter, indenting levels.</li>
  <li>Consider removing TextEdit from list of editors, as it has a tendency to not save in plain text (and confuse students greatly).</li>
  <li>Show how to debug HTML in Firebug and Chrome developer console (element/DOM tab).</li>
  <li>Re-iterate that the title element goes in the head and is not rendered on the page (this seems a matter of great confusion for newbies).</li>
  <li>Consider talking about the HTML as a tree structure (DOM).</li>
</ul>

### HTML: Exercise
Create a webpage using only HTML that touches on all of the parts of HTML discussed above. 
