---
layout: post
title: "Finally on the Octopress"
date: 2012-06-11 10:59
comments: true
categories: octopress
---

I'm finally able to post on Octopress! Woohoo!

The directions to create the site were pretty straight forward, but I had some trouble getting Octopress to catch my blog post.

<hr>

### Step 1
{% codeblock lang:rb %}
rake new_post["this is the title of the post"]
{% endcodeblock %}

This creates the new post.

### Step 2
{% codeblock lang:rb %}
git add .
git commit -m 'your message here.'
git push origin source # make sure you add 'origin source' or it will yell at you.
{% endcodeblock %}
The weird thing is that you won't see any changes to your github repo. (Until after step 4)

### Step 3
{% codeblock lang:rb %}
rake generate
{% endcodeblock %}
This step creates the html blog doing some kind of github pages magic behind the scenes.

### Step 4
{% codeblock lang:rb %}
rake deploy
{% endcodeblock %}
This actually sends the files to github, and to your blog address.