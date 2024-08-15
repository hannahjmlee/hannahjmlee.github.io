---
layout: page
permalink: /repositories/
title: repositories
description: Explore my public GitHub repositories, where I share the code underlying my research and publications in multi-robot coordination. Feel free to use the code, and don’t hesitate to reach out if you have any questions! My Multi-Agent Navigation Algorithms (MANA) libraries are central to my research. MANA-Labs is a Python library designed for the rapid development and experimentation of new algorithms. While the code in MANA-Labs is more experimental and less optimized, it’s a great resource for exploring novel ideas. MANA-Core, written in C++, focuses on testing and evaluating algorithms. Though it supports fewer algorithms, MANA-Core features clean, optimized code for efficient and reliable experiments.
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
