---
layout: page
title: Ecosystem
permalink: /ecosystem/
categories: main-nav
---

This page offers an overview of the people and organizations influencing the future of law.



{% comment %}
This is a list of organizations. If you want yours to be included, include "org" in the front matter tags on your page
{% endcomment %}

<h3>Organizations</h3>
<ul>
	{% for page in site.pages %}
		{% if page.tags contains "org" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>

