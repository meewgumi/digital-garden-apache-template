---
layout: page
title: Archive
---
# Archive
<ul class="archive">
{% for note in site.notes %}
<li><a href="{{ note.url }}{%- if site.use_html_extension -%}.html{%- endif -%}" class="internal-link">{{note.title}}</a>{% if note.theme != null %} in {{note.theme}}{% endif %} <span>({{ note.last_modified_at | date: "%B %Y" }})</span>{{ note.excerpt }}</li>
{% endfor %}
</ul>
