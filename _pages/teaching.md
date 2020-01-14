---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

{% include base_path %}


<h2 class="archive__subtitle" itemprop="headline"> Current </h2>
{% for post in site.teaching %}
	{%if post.semester == 'Fall 2019' %}
		{% include archive-single.html %}
	{%endif%}
{% endfor %}

<h2 class="archive__subtitle" itemprop="headline"> Previous </h2>
{% for post in site.teaching reversed %}
	{%if post.semester != 'Fall 2019' %}
		{% include archive-single.html %}
	{%endif%}
{% endfor %}
