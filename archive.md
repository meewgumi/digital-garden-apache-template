---
layout: page
title: Archive
nav_item: true
---
# Archive
## Notes
<ul>
{% for note in site.notes %}
<li><a href="{{ note.url }}{%- if site.use_html_extension -%}.html{%- endif -%}" class="internal-link">{{note.title}}</a> - {{ note.last_modified_at | date: "%B %-d, %Y" }}</li>
{% endfor %}
</ul>
