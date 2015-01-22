# Week 2 Review
A review of topics chosen by you during week 2! (rhyming intentional)
#Objectives
* Understand the return statement within a function
* Be comfortable searching for and reading Docs
* Understand the use of a callback within iterators
* Be comfortable with reimplementing your own iterator (map)
* Understanding why we use the TDD style
* Be comfortable reading tests written with Mocha / Chai
* Understand "Setup, Exercise, Verify"
* Understand how to read your errors
  

&nbsp;

##Docs, Return, & Iterators
###Basic Definitions
* **Docs** (Documentation): When we reference the docs, we are referring to the documentation of a given language, library, framework, etc... 
	* Javascript: [https://developer.mozilla.org/en-US/docs/Web/JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
	* Bootstrap: [http://getbootstrap.com/getting-started/](http://getbootstrap.com/getting-started/)	
* **Iterator**: An Iterator is an object (read: function) that knows how to access items from a collection one at a time, while keeping track of its current position within that sequence.

###Return
#####So... why do we use return?
Here it is important for us to first think about the underlying environment we are using the return statement in: a function.

When a function is invoked, it begins execution with the first statement , and ends when it hits the } that closes the function body. That causes the function to *return* control to the part of the program that invoked the function.

Now, here's where it gets tricky, a function in javascript always 
returns a value. It just doesn't implicitly return the last line of the function like some other nifty languages ::cough:: ruby ::cough, cough:: So, in javascript, if the return value is not specified, then *undefined* is returned. Thus, we designate a return statement inside our function to return the value we would like the function to pass to the program that invoked it.

#####But what does it actually do?
A return is a statement that we use within functions to cause a function to *return* early. When return is executed, the function returns immediately without executing the remaining statements. **

#####Wait...didn't we use two returns that one time?
We did. Let's parse through this bad boy together. 
 
```javascript
function tripler (numbers) {
    return numbers.map(function(num) {
      return num * 3;
    });
  }
```
###Docs & Iterators
So we just looked at map from a use case standpoint, lets give reimplementing it a whirl. 

Let's take a look at the docs together. To do this, we've provided a link below that outlines a good workflow for finding some docs...

* <a href="http://lmgtfy.com/?q=javascript+map+mdn" target="_blank">Click me!</a>

#####Steps:
1. Pair with the person next to you
2. Discuss your understanding of the documentation we just read
3. Use a pencil and paper // whiteboard marker to psuedo-code what you're about to do
4. Write some code. Have one pilot (typing) & one navigator (observe,comment,debug) - *Remember your etiquette - don't interrupt a thought,  don't interrupt a line of code being written (typos can be fixed at the end), use good tone, every idea merits discussion.* 


