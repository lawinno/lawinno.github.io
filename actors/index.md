---
layout: page
title: Actors
permalink: /actors/
categories: main-nav
---

This page offers an overview of the people and organizations influencing the future of law through action.

{% comment %}
This is a list of organizations. If you want yours to be included, include "org" in the front matter tags on your page
{% endcomment %}

<h3>Non-profits and informal groups</h3>
<ul>
	{% for page in site.pages %}
		{% if page.tags contains "org" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>

<h3>Startups</h3>
<ul>
	{% for page in site.pages %}
		{% if page.tags contains "startup" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>


<h3>Established Companies</h3>
<ul>
	{% for page in site.pages %}
		{% if page.tags contains "big-company" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>


<h3>People</h3>
<ul>
	{% for page in site.pages %}
		{% if page.categories contains "people-class" %}
			<li>
				<a href="{{ page.url }}">{{ page.title }}</a>: {{ page.short-description }}
			</li>
		{% endif %}
	{% endfor %}
</ul>


