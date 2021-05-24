---
layout: page
title: Archive
---
# Archive
## Pages
<ul>
{% for page in site.pages %}
    <li><a href="{{ page.url | relative_url }}{%- if site.use_html_extension -%}.html{%- endif -%}" class="internal-link">{{ page.title }}</a></li>
    {% endfor %}
</ul>
## Notes
<ul>
{% for note in site.notes %}
<li><a href="{{ note.url }}{%- if site.use_html_extension -%}.html{%- endif -%}" class="internal-link">{{note.title}}</a> - {{ note.last_modified_at | date: "%B %-d, %Y" }}</li>
{% endfor %}
</ul>
