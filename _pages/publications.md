---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

### [Conference Papers](#conferences) &nbsp;&nbsp;&nbsp; [Journal Articles and Book Chapters](#journals) &nbsp;&nbsp;&nbsp; [External References](#external)

<h2 name='conferences'> Conference Papers </h2>

{% capture written_year %}'None'{% endcapture %}
{% for post in site.publications reversed %}
  {% if post.type != 'journal' %}
    {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
    {% if year != written_year %}
      {% include year-heading.html %}
      {% capture written_year %}{{ year }}{% endcapture %}    
    {% endif %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


<h2 name='journals'> Journal Articles and Book Chapters </h2>

{% capture written_year %}'None'{% endcapture %}
{% for post in site.publications reversed %}
  {% if post.type %}
   {% if post.type == 'journal' %}
    {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
    {% if year != written_year %}
      {% include year-heading.html %}
      {% capture written_year %}{{ year }}{% endcapture %}    
    {% endif %}
    {% include archive-single.html %}
   {% endif %}
  {% endif %}
{% endfor %}

<h2 name='external'> External Reference Sources </h2>
{% include pubs_header.md %}
