---
layout: default
title: Seminar Repos
---

{% assign sorted_public_repositories = site.github.public_repositories | sort_natural: "name" %}

# BCBB Training Seminar GitHub Repositories

These are the GitHub repos with all of the classroom scripts and notes for each of the classes:

{% for repository in sorted_public_repositories %}
  {% if site.data.repos contains repository.name %}

  - [{{ repository.name }}]({{ repository.html_url }})

     {{ repository.description }}

	{% endif %}

{% endfor %}

