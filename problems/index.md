---
layout: page
title: Problems
permalink: /problems/
categories: main-nav
---

<h2>Problems</h2>

This page collects some of the problems affecting the legal community, which innovation should aim to solve.

<ul>
	{% for page in site.pages %}
		{% if page.categories == "problems" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>