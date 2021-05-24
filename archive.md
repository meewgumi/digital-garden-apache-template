---
layout: page
title: Archive
---
# Archive
## Notes
<ul>
{% for note in site.notes %}
<li><a href="{{ note.url }}{%- if site.use_html_extension -%}.html{%- endif -%}" class="internal-link">{{note.title}}</a> - {{ note.last_modified_at | date: "%B %-d, %Y" }}</li>
{% endfor %}
</ul>

{% if note.category == "Cats" %}
### Cats
  {% for note in site.notes %}[{{note.title}}]({{note.url}}){% endfor %}
{% elsif note.category == "Getting Started" %}
### Getting Started
  {% for note in site.notes %}[{{note.title}}]({{note.url}}){% endfor %}
{% else %}
### Uncategorized
  {% for note in site.notes %}[{{note.title}}]({{note.url}}){% endfor %}
{% endif %}
