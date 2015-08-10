Lesson 2 - Outputting Text To The Web Page
===========================================

In your previous JavaScript tutorials you have used console.log to output text like this:

```javascript 
console.log("Hello World!"); 	 
```
← [RUN](http://jsbin.com/suwaracaqu/1/edit?js,console) this to see it in action if you like

Or using this:
```javascript
window.alert("Hello World!");  	
```
← Which works from a web page [POP-UP](http://jsbin.com/yinenirore/1/edit?html,output) - (click “Run with JS”)
```html
<html>
	<body>
		<script type='text/javascript'>
			window.alert("Hello World!");
		</script>
	</body>
</html>
```
However, this only outputs to a console (or terminal) used for testing your code and not to the screen or a web page.  To do that we use a different command:
```javascript
document.write("");	
```
By adding your name between the quotes it now appears on the web page.

Exercise
```html
<html>
  <body>
    <script type='text/javascript'>
      document.write("");
    </script>
  </body>
</html>
```
Using this method we can also output variables and strings.

Exercise: Add Some Variables

[TRY](http://jsbin.com/kodubupatu/1/edit?html,output) adding a variable for your name and your age and outputting it using document.write.

Note: you need to put a comma between the name and age to separate them.

If you have any trouble doing this 	

→ [HERE](http://jsbin.com/dujenamila/1/edit?html,output) is an example for you to fill out.

```html
<html>
  <body>
    <script type='text/javascript'>
      var name = "";
      var age = 0;
      document.write(name, age);
    </script>
  </body>
</html>
```
Exercise: Format Your Output

However, this doesn’t quite look so tidy, so why don’t you [ADD](http://jsbin.com/difowucoci/1/edit?html,output) a comma and some spacing between the name and age.  To do this just add some quotes containing this in between.

Not sure how to do this?	→ [LOOK](http://jsbin.com/balihuqixi/1/edit?html,output) at this example, add your name and age
```html
<html>
  <body>
    <script type='text/javascript'>
      var name = "";
      var age = 0;
      document.write(name, ", ", age);
    </script>
  </body>
</html>
```
Note: Notice how we needed to add the spacing and comma inside quotes to make it appear on the page, and also needed commas around it to separate it from the variables.
