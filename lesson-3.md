Lesson 3 - Accepting Input From A Web Page
===========================================

This tutorial presumes you have already learnt how to do web forms.  If not [here is Code Academy’s interactive tutorial](http://www.codecademy.com/courses/web-beginner-en-Vfmnp/0/1) on the subject.

In your previous JavaScript tutorials you have used prompt to input text like this:
```javascript
var reply = prompt("What’s your name? ");  
```
Surprise - this works with web pages too!  We can add a line to output the results thus:
```javascript
document.write(“Hello “, reply);
```
← [HERE](http://jsbin.com/jebudateso/1/edit?html,output) You can see it all work

However, there are more elegant ways to get input from a web page.  We can create an input form field in HTML like this:
```html
<input type="text" id="myText" value="Sample text">		
```
← [TRY](http://jsbin.com/huyaqelebo/1/edit?html,output) this

But, this only accepts the text input though and it doesn’t put it in a variable, nor does it submit it in any way.  This where things get a little more complicated, but don’t worry we’ll break it down step by step.

**Exercise: Form Based Text Input**

Starting with a basic web template …	← [OPEN](http://jsbin.com/cekigaluwe/1/edit?html,output) a basic page for editing
... lets create the HTML form with the input in it.  Put the following in the `<body>` of the page:
```html
    <form name="testForm" onsubmit="return processForm()"> 
      Type something: 
      <input name="aTextField" value=""> 
      <input type="submit" value="Then click me"> 
    </form> 
```
This creates a form, tells the user to type something, add an input box, and ends with a submit button.

When submitted this form calls the processForm function - so we need to create that. …

Put this function in the `<head>` of the page:
```javascript
    function processForm() { 
      var fieldVal = document.testForm.aTextField.value; 
      document.write("You typed: " + fieldVal); 
      return false;  
    } 
```
← [TRY](http://jsbin.com/hobaxumeri/1/edit?html,output) this out for yourself (if yours doesn’t work)

This function creates a variable from the text input field in the form, then it displays this variable.

So what is the “return false” statement for?  It just lets the page know it doesn’t need to ask again for the text input.

Lesson 4 - Outputting Text To A Specific Element In A Web Page