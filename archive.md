---
layout: page
title: Archive
---
# Archive
## Pages
<ul>
{% for page in site.pages %}
    <li><a href="{{ page.url | absolute_url }}">{{ page.title }}</a></li>
    {% endfor %}
</ul>
## Notes
<ul>
{% for note in site.notes %}
<li><a href="{{ note.url }}">{{note.title}}</a> - {{ note.last_modified_at | date: "%B %-d, %Y" }}</li>
{% endfor %}
</ul>
