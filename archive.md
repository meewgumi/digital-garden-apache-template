---
layout: page
title: Archive
---
# Archive
## Pages
<ul>
{% for page in mypages %}
    <li><a href="{{ page.url | absolute_url }}">{{ page.title }}</a></li>
    {% endfor %}
</ul>
## Notes
<ul>
{% for note in site.notes %}
<li><a href="{{ notes.url }}">{{note.title}}</a> - {{note.last\_modified\_at | date: "%Y-%m-%d"}}</li>
{% endfor %}
</ul>
