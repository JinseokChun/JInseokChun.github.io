---
layout: page
title: Projects
permalink: /projects/
description: Research projects I take part in.
nav: true
nav_order: 2
---

<!-- pages/projects.md: one card per project in _projects/, ordered by `importance` -->

{% assign sorted_projects = site.projects | sort: "importance" %}

<div class="project-list">
{% for project in sorted_projects %}
  <div class="project-card">
    {% if project.logo %}
      <div class="project-card-logo">
        <img src="{{ project.logo | relative_url }}" alt="{{ project.logo_alt | default: project.funding }}" loading="lazy">
      </div>
    {% endif %}
    <div class="project-card-body">
      <h2 class="project-card-title">{{ project.title }}</h2>
      {% if project.funding %}<p class="project-card-funding">{{ project.funding }}</p>{% endif %}
      {% if project.period %}<p class="project-card-period">{{ project.period }}</p>{% endif %}
      {% if project.role %}<p class="project-card-role">{{ project.role }}</p>{% endif %}
    </div>
  </div>
{% endfor %}
</div>
