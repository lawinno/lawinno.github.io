---
layout: page
title: Ideas
permalink: /ideas/
categories: main-nav
---

<h2>Ideas</h2>

This page collects some of the concepts driving change in the legal field.

<ul>
	{% for page in site.pages %}
		{% if page.categories == "ideas" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>
