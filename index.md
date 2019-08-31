# Welcome to the BCBB Training Seminars!

Here's a list of the seminars:

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }}) - {{ repository.teams_url }}
{% endfor %}
