---
layout: default
---

# Welcome to the BCBB Training Seminars!

Here's a list of the seminars:

{% for repository in site.github.public_repositories %}
  {% if repository.topics contains 'bcbb-training' %}
  - [{{ repository.name }}]({{ repository.html_url }})
	
	{% endif %}

{% endfor %}
