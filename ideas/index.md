---
layout: page
title: Ideas
permalink: /ideas/
categories: main-nav
---

This page collects some of the concepts driving change in the legal field.
<hr>

<ul>
	{% for page in site.pages %}
		{% if page.categories contains "ideas" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>
