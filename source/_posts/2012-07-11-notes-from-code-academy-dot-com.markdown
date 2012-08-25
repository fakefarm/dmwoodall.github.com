---
layout: post
title: "Notes from Code Academy dot com"
date: 2012-07-11 08:43
comments: true
categories: javascript
---
I started [CodeAcademy.com](http://CodeAcademy.com/) yesterday to learn JavaScript. Couple things that I wanted to record;

###syntax
JavaScript, needs extra syntax to work. Things such as semi-colons, the word var, and braces. JavaScript is also case sensitive.

###naming a variable
I need to add the word 'var' to describe a variable, and add the semi-colon at the end. It's taken a little getting used to.

{% codeblock %}
// An example; 
var name = "Dave"
{% endcodeblock %}

###naming a function
To create a function you do it the same by calling;

An Example;
var printReport = function(){
  ...
};
the semi-colon doesn't show up until the end of the function.


###for loops
Creating a for loop needs to declare three things;

{% codeblock %}
// An example; 
for(i = 0; i <= 10; i++){
  // code here
};
{% endcodeblock %}

Sets that tripped me up at first
1. i is the variable incrementor.
2. Set i to some value
3. Then add a semi-colon!
4. Set the height to the incrementor (i)
5. Then add a semi-colon!
6. Set the incrementor as a ++, which is a shorthand of saying "Add 1"

