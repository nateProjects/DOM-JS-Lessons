Lesson 1 - Including JavaScript In A Web Page
==============================================

One difference with using JavaScript in a web page is that you have to let the web page know when you are ‘speaking’ in JavaScript.  The simplest way is to include it like this -
```html
<script type='text/javascript'>
// Your script goes here.
</script>
```
In the middle of a web page it would look like this:
```html
<html>
  <body>
    <script type='text/javascript'>
      // Your script goes here.
    </script>
  </body>
</html>
```

At the moment as you can see this doesn’t output anything, but it doesn’t come up with any errors either.  It is just waiting for you to add any JavaScript code you want between the `<script>` tags.

It is also possible to write JavaScript in a different file and include it within your web page.  To do so you’d write something like the line below:
```html
<script type='text/javascript' src='source.js'></script>
```

As well as Javascript, CSS styles can also be added in an external file:
```html
<head>
	<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

[Lesson 2 - Outputting Text To The Web Page](lesson-2.md)