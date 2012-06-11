---
layout: post
title: "adding a code block"
date: 2012-06-11 11:20
comments: true
categories: octopress
---

I was reading the [Octopress Documentation]("http://octopress.org/docs/plugins/codeblock/") about code blocks and decided to try it here;

{% codeblock working on this technical blog lang:rb http://app/controllers/application_controller.rb Example application controller %}

class ApplicationController < ActionController::Base
  protect_from_forgery
end

{% endcodeblock %}