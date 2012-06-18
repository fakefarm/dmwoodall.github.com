---
layout: post
title: "ruby instance variables"
date: 2012-06-12 09:35
comments: true
categories: Well Grounded Rubyist, Ruby Syntax
---

Did you know that a Class can also call on it's own instance variables?

{% codeblock While reading "Well Grounded Rubyist" lang:rb http://app/controllers/application_controller.rb Classes using Instance Methods %}
class TheClass
	puts "Just inside class definition block. Here's self:"
	puts self
	# ---------------------
	@instance_variable = "I am an instance variable at the top level of a class body."
	puts "And here's the instance variable @v, belonging to #{self};"
	# ---------------------
	p @instance_variable

	def object_method
		puts "Inside an instance method def block. Here's self:"
		puts self.clean_name # notice that self has now changed to reference the object

		puts "And here's the instance variable @instance_variable, belonging to #{self.clean_name}"
		puts @instance_variable #this will return nil, because it hasn't been defined within the object's scope.
	end	
	
	def clean_name
		"Mr. Object"	
	end
end

# This is where we call on the class and methods;

c = TheClass.new
c.show_variable

{% endcodeblock %}
