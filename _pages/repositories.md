---
layout: page
permalink: /repositories/
title: repositories
description: Explore my public GitHub repositories, where you'll find code supporting my publications and advancements in multi-robot coordination. You're welcome to use any of the shared code, and please don't hesitate to contact me with any questions!
nav: true
nav_order: 4
---

## GitHub Repositories

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
