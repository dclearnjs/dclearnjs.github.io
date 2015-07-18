---
layout: post
title:  "Fundamentals of JavaScript"
date:   2015-06-07 15:03:08
categories: javascript
---

# Fundamentals of JavaScript  

JavaScript was originally called LiveScript, but changed to JavaScript for marketing purposes. The programming language Java was really big at the time, and LiveScript marketers wanted to ride that wave. Java and JavaScript have very little in common. Java is what powers a lot of software and android apps. JavaScript is what is used to add interactivity to the browser.  JavaScript can now be used outside of the browser, or on the server, thanks to frameworks like Node.js.  

Some people might refer to other frameworks or libraries like Ember, Backbone, Angular, or any number of other frameworks. Frameworks and libraries are usually open-source (built for free, to be used for free) code projects that anyone can contribute to, and anyone can use. They are built to address certain problems someone might be facing or fix something someone thinks is wrong in another framework.JavaScript has a very active community that is constantly working to create new and improve older frameworks.

You can write JavaScript directly into the browser by right-clicking on a page and going to “inspect element” - this will show you the code for everything that is on the page. Go to the “console” tab and you will be able to evaluate JavaScript you type in directly. This is useful for playing around with it. If you want to write a JavaScript program and use it later, you would use a text editor like Sublime Text or you can use Codepen or JSFiddle, or a browser based development environment like Coud9. 

## Values
JavaScript is built on values. There are different types of values:
Strings
Numbers
booleans

Values are the basic building blocks of JavaScript. 

### Numbers 

Expressed in JS as :

12 

or 

3.5 or 

3.0e6 

You can use operators such as +, -, *, /, or % to perform arithmetic on a number.

3 + 9

23 - 5 * 34

5 % 6

Operators follow order of precedence, or PEMDAS. % (modulo or remainder) follows same precedence as multiplication and division. 

### Strings

Strings are a set of characters. Enclose the contents of the strings in quotation marks. You can use either “   “ or ‘   ‘ as long as the closing and ending match.

“This is a string.”
‘This is also a string!’
“1 more string.”

Escape characters that you cannot include in the one line. \n for new line, and \’ to escape a quote mark. 

Using the + operator concatenates the string.

“c” + “a” + “t” 
“cat”

“5” + “4”
“54”

### Booleans:

This is on/off, yes/no and other binary options expressed as either true or false. Think checkbox when signing up for a website agreeing to ToS.

_Comparisons_

console.log(3 > 2)
=> true
console.log(5 < 4)
=> false

>=  greater than or equal to
<= less than or equal to
!= not equal to

_Logical operators _

&&  this means ‘and” in the logical sense. This AND that.
| |  this means ‘or’ in the logical sense. This OR that.
!   this means ‘not’ in the logical sense. !true = false.
 
console.log( (4 > 3) && (5 < 6) )
=> true

Using  || will evaluate to true if either one of the statements is true. 
console.log( (4 > 3) ||  (5 >6) )
=> true

## Structure

### Variables
Ways of keeping/storing data. use lower-camel-case by convention. You can create variable names in all lowercase if you would like, but this is the convention most people use and understand. Try to keep variable names clear and concise. var a might be concise, but it’s not very clear. thisVariableIsForDeterminingTheSumOfTwoPlusTwo is clear, but not concise. Variable names cannot start with a digit but a digit can be included. Two variables can have the same value, and a variable’s value can change later. Variables can hold all types of values: strings, booleans, numbers, and even functions.

Expressed in JS as:

var catsAreCool = “cats are cool”
var myNumber = 5 * 4
var printCats = console.log(“cats”)

You can call a variable later to access the value inside of it.

### Functions
Functions are bits of reusable code you can call later in a program.   

function myFunction(parameter1, parameter2) {  
	return parameter1 + parameter2;  
};  

You start the function by denoting it’s a function, then you give it a name, using the same naming convention you used in naming variables. Inside of the the parenthesis you would put parameters, or arguments. This is something you might want to pass to the code late. Inside of the curly braces you want to put the code you want to be able to do. You end by adding a semicolon, which tells it you have ended your statement, it’s like a period at the end of a sentence in English Later you can call the function with the parameters you want to pass it, and it will execute it.  

myFunction(1, 3)  
=> 4  

A note about syntax: syntax is those curly braces and parentheses and other rules about punctuation in JavaScript. JavaScript is not white space sensitive, meaning adding spaces or line breaks doesn’t change how the code runs. You could also write the function like this:  

function myFunction(parameter1, parameter2) {return parameter1 + parameter2;};  

Adding in spaces and line breaks makes the code more readable for the humans reading the code. You are always writing code for both the computer and a human, that human is usually you four months down the line, so be clear!  

### If/Else

You can use If  / Else to only run certain bits of code if certain conditions are met. This is called control flow. 

if (condition ) {  
	code you want to run if condition is true;  
}  

You can use the if statement by itself, or you can add an else statement.  

if (condition) {  
	code you want to run if the condition is true;  
} else {  
	code you want to run if the condition is false;  
};  

This syntax is similar to the function syntax, with () encapsulating your parameters or arguments, and {} containing the code you want to run. ; again ends the statement. You could write this all as one line, too.  

var myPet = “cat”  
if (myPet = “cat”) {  
	return “meow”;  
} else {  
	return “that is not a cat”;  
};  

### Loops