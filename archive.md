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

{% for note in site.notes %}
{% if category == "Cats" %}
### Cats
  [{{note.title}}]({{note.url}})
{% elsif category == "Getting Started" %}
### Getting Started
  [{{note.title}}]({{note.url}})
{% else %}
  ### Uncategorized
  [{{note.title}}]({{note.url}})
{% endif %}
{% endfor %}
