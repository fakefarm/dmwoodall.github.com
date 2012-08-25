---
layout: post
title: "html-forms"
date: 2012-07-19 12:42
comments: true
categories: html, forms
---

Treehouse is so well organized that I'm taking the time to review the fundamentals. Over the past two years I've consumed several blogs, books, videos, and talks but I know it didn't all sink in. Through Treehouse's quizzes and challenges I'm able to see where the gaps are.

Reviewing their [html badge](http://teamtreehouse.com/library/design-foundations/html) how little I knew about forms. Here are my notes from [forms badge](http://teamtreehouse.com/library/design-foundations/html/forms). A form will have the following format;

{% codeblock %}
<form action="#" method="POST" name="my Form">
  <input type='text' name='username'>
  <input type='submit'>
</form>
{% endcodeblock %}

####Action
Where you send the form once it's submitted.

####Method
This refers to HTTP GET, POST, PUT, DELETE

####Name
Name of the form

####Type
Type is the aspect you add to the form to instruct what type of input field you want. Most popular are 'text', 'radio', 'checkbox'

####Text Area
Use textarea when you want a larger typing area for something like comments. 

{% codeblock %}
<textarea name="essay" rows="10" cols="30"></textarea>
{% endcodeblock %}

####Select
For creating dropdown lists. Good when there are a lot of options. 

{% codeblock %}
<select>
  <optgroup label="Americas">
    <option>North America</option>
    <option>South America</option>
  </optgroup>
  <optgroup label="Americas">
    <option>Europe</option>
    <option>Europe</option>
  </optgroup>
</select>
{% endcodeblock %}

<optgroup> is for organizing drop downs and making non-selectable categories. Very nice!
  
####Name
Name is important for grouping items together. For example, if you have two radio buttons, the similar name will cluster them together.

####Value 
Value relates to server side programming to know how to store these items.

####Labels

####Fieldset & Legend
Use <fieldset> to organize the and surround with a border form.
Use <legend> to provide a title on that same information.
Pass a center if you want to align; <legend align="center">

 