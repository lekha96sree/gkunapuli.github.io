---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include pubs_header.md %}

{% include base_path %}


{{ <h2> Journal Articles and Book Chapters </h2> }}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.journals reversed %}
  {% if post.type == 'journal' %}
    {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
    {% if year != written_year %}
      {% include year-heading.html %}
      {% capture written_year %}{{ year }}{% endcapture %}    
    {% endif %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
