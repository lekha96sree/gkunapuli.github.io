---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include pubs_header.md %}

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.publications reversed %}
{% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    {% include year-heading.html %}
    {% capture written_year %}{{ year }}{% endcapture %}
    {{ post.collection }}
    {% if post.collection == 'journals' %}
    JOURNAL
    {% endif %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}
