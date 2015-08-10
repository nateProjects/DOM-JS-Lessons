Lesson 4 - Outputting Text To A Specific Element In A Web Page
===============================================================

What if you want your text to appear in a particular paragraph or part of a web page?
```html
<p id="test">text</p>
<script type='text/javascript'>
document.getElementById("test").innerHTML = "Hello World!";
</script>
```
[TYPE](http://jsbin.com/rimewivero/1/edit?html,output) this in yourself or [WATCH](http://jsbin.com/qebuqiconi/1/edit?html,output) it in action (if yours doesn’t work)

Notice that the new text overwrote the old text!  In fact it did it so fast you didn’t even see the old text at all!

Let’s break this down so it’s not so complex -

Code			|	Explanation
----------------|---------------------------------------------------------------------------
document. 		|	← this is what you are working on - the document or web page
getElementById	|	← this is how we are getting what you want to change or add to
			    |	 (we are getting an element of the web page defined by an “id”)
("test"). 		|	← this is the name of the “id” we are changing or adding to
innerHTML 		|	← this is how we are replacing it - using HTML
			    |	(alternatively we could have used “innerText” if just altering the text)

**Exercise: Change The Text In A Heading**

[HERE](http://jsbin.com/naqanijeke/1/edit?html,output) is a basic HTML page with a heading.  Change the heading so that it says something different.  Don’t forget to name the “id” and add the text.

**Exercise: Output Form Based Input To The Same Page**

This concept works with input too - In the previous section the page refreshed when someone entered their name - But what if we wanted to do it on the same screen without refreshing the page?

Lets [START](http://jsbin.com/wutehucoba/1/edit?html,output) with the old input page we created …

On the line below the </form> tag add a paragraph with the id “showText” -
```html
<p id="showText"></p> 
```
In the JavaScript at the top of the page change this line -
```javascript
document.write("You typed: " + fieldVal);
```
… which previously printed your input to a new page to -
```javascript
document.getElementById("showText").innerHTML = "You typed: " + fieldVal;
```
← [HERE](http://jsbin.com/weqihiquju/1/edit?html,output) is a completed version to look at

Using elements like this is a better way to place text, but it is still limited.  Sometimes we need to control exactly where our text is. ...  

Lesson 5 - Placing Text On A Web Page Using CSS