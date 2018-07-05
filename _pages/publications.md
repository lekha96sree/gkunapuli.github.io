---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

### [Conference Papers](#conference-papers) &nbsp;&nbsp;&nbsp; [Journal Articles and Book Chapters](#journal-articles-and-book-chapters) &nbsp;&nbsp;&nbsp; [External References](#external-references)
=====

## Conference Papers
--------------------

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


## Journal Articles and Book Chapters

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

## External References
{% include pubs_header.md %}
