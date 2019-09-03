---
layout: default
title: Home
---

{% assign sorted_public_repositories = site.github.public_repositories | sort_natural: "name" %}

# Welcome to the BCBB Training Seminars!

Here's a list of the seminars:

{% for repository in sorted_public_repositories %}
  {% if site.data.repos contains repository.name %}

  - [{{ repository.name }}]({{ repository.html_url }})

     {{ repository.description }}

	{% endif %}

{% endfor %}

