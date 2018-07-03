---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can also find my articles on <u><a href="https://scholar.google.com/citations?user=XewwOE8AAAAJ&hl=en">my Google Scholar profile</a>.</u>

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.publications reversed %}
{% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    {{ year }}
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}
