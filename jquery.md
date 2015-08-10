JQuery Overview
================

**Including The JQuery Library**
```html
<script src="http://code.jquery.com/jquery-latest.min.js" type="text/javascript">
</script>
```
**Using JQuery Within A Web Page**
```javascript
$(document).ready(function(){
	/* html of page exists now, run jQuery here */
});
```
**Outputting Text To The Web Page**
```html
<p></p>
 <script>
	$( "p" ).text( "Some new text." );
</script>
```html
**Placing Text On A Web Page Using CSS**
```html
<p id=”thisParagraph”></p>
 	<script>
$( "#thisParagraph" ).text( "Some newer text." );
</script>
```
[HERE](http://jsbin.com/qovezokexo/1/edit?html,output) you can see a page that includes example of all of these.

**Further Progress**

To follow a step by step interactive tutorial on JQuery you can go to -

http://www.codecademy.com/tracks/jquery (3 hrs)

Other courses include -

* [Code School](https://www.codeschool.com/courses/try-jquery)
* [w3 Schools](http://www.w3schools.com/jquery/default.asp)
* [Tuts+](http://code.tutsplus.com/courses/30-days-to-learn-jquery)
* [After Hours](http://www.afterhoursprogramming.com/tutorial/JavaScript/jQuery-Introduction/)
* [Cheat Sheet](http://overapi.com/jquery/)
