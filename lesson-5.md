Lesson 5 - Placing Text On A Web Page Using CSS
================================================

What if we wanted to put some text wherever we wanted?  In this section we will learn to marry JavaScript and CSS so that we can pick the exact point we want to output to on the screen.

**CSS - A Refresher**

CSS is HTML with style!  It is the way we specify what part of the page we want to use, what color it is, and what formatting the text takes on.  CSS can be embedded in paragraph’s, headings, divisions and just about any element:
```html
<h1 style="color:blue; margin-left:30px;">This is a heading.</h1>
```
It can also be used to rewrite how all HTML tags appear on the page, or only specific ones:
```html
<style>
	body {
    	background-color: linen;
	}
#myLine {
		color: maroon;
		margin-left: 40px;
	} 
</style>
```
**Exercise: Place Text In A CSS Styled Element**

[TRY](http://jsbin.com/wuruxepele/1/edit?html,output) putting the above CSS code in the head of a web page and creating a paragraph to use it.  If your text doesn’t turn maroon [LOOK](http://jsbin.com/qisiyosaqu/1/edit?html,output) at this example and see why.

**Exercise: Change The Style In An Element**

Using innerHTML you can change the style of text too:
```javascript
document.getElementById("test").innerHTML = "<b>Hello World!</b>";
```
← [SEE](http://jsbin.com/mojovaxuyi/1/edit?html,output) this in action.  Try and add some internal CSS to it.

**Reminder: External CSS Files**

Note: If we are making enough changes to our styles we can use an CSS external file -
```html
<head>
	<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```
[Lesson 6 - Placing Images On A Web Page Using CSS](lesson-6.md)
