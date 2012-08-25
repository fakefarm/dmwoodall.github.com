---
layout: post
title: "CSS3 Selectors"
date: 2012-07-20 17:19
comments: true
categories: CSS
---

Notes from ["CSS Selectors"]("http://teamtreehouse.com/library/design-foundations/css3/selectors"). 

##Attribute Selectors

{% codeblock %}
img[src^="images"]{
  border: 5px solid orange;
}
{% endcodeblock %}
^ is looking for any image tags that have a source attribute that begins with exact string "images"

{% codeblock %}

img[src$=".jpg"]{
  border: 5px solid green;
}
{% endcodeblock %}
$ is looking for any image tags that have a source attribute that ends with exact string ".jpg"


a[href*="#"]{
  border: 5px solid orange;
}
{% endcodeblock %}

selecting all 'a' tags that have href attributes that contain exact sub-string.

##Pseudo Classes

:root{
  background: orange;
}

####Nth-Child()

{% codeblock %}
#nav li:nth-child(1){
  border: 5px solid orange;
}
{% endcodeblock %}
Useful for selecting any children, by number

####nth-last-child()
goes to the last child, and counts backwards.


####nth-of-type
Allows you to select based on the type - (class 'post' for example.)

{% codeblock %}
#content .post:nth-of-type(2){
  background: orange;
}
{% endcodeblock %}


####nth-last-of-type()
counts backwards


####last-child()
a CSS2 feature, but one to notice.


####first-of-type()
same as nth-of-type(1)

####last-of-type

####only-child

{% codeblock %}
.header h1:only-child{
  background:orange;
}
{% endcodeblock %}
Only selects groupings that have a single child element.

####only-of-type
{% codeblock %}
.header h1:only-of-type{
  background:orange;
}
{% endcodeblock %}

####empty


{% codeblock %}
.header:empty{
  background: orange;
  width: 200px;
  height: 200px;
  display:block;
}
{% endcodeblock %}

##Miscellaneous Selectors

####Target pseudo class

{% codeblock %}
#poll:target{
  
}
{% endcodeblock %}
Once you click on the target, once it's highlighted it will activate.

####Enabled

####checked
shows when a button is being selected. (Can't change the background color for some reason...)

{% codeblock %}
#poll input:checked{
  width:30px;
}
{% endcodeblock %}

####Negate
Select radio buttons that are not checked.

{% codeblock %}
#poll input:not(:checked){
  
}
{% endcodeblock %}

####General Sibling combinator

{% codeblock %}
ul ~ #sidebar{
  background: orange;
}
{% endcodeblock %}

~ character - anything comes after is the sibling that will actually be selected.
the part that comes before the "~" is a sibling that came previously. 