---
layout: page
title: Blog
permalink: /blog/
---

Here are all the blog posts

<ul>

	{% for post in site.posts %}
		<li><a href="{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}

</ul>