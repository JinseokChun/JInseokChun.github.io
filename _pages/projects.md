---
layout: page
title: Projects
permalink: /projects/
description: Research projects I take part in.
nav: true
nav_order: 2
---

<!-- pages/projects.md: every project in _projects/ is shown in full here, ordered by `importance` -->

{% assign sorted_projects = site.projects | sort: "importance" %}

<div class="project-list">
{% for project in sorted_projects %}
  <section class="project-entry">
    {% if project.logo %}
      <div class="project-logo">
        <img src="{{ project.logo | relative_url }}" alt="{{ project.logo_alt | default: project.funding }}" loading="lazy">
      </div>
    {% endif %}

    <h2 class="project-title">{{ project.title }}</h2>
    {% if project.title_ko %}
      <p class="project-title-ko" lang="ko">{{ project.title_ko }}</p>
    {% endif %}

    {% if project.funding %}
      <p class="project-funding"><i class="fa-solid fa-landmark"></i> Funded by {{ project.funding }}</p>
    {% endif %}

    <div class="project-body">
      {{ project.content | markdownify }}
    </div>

    {% if project.tags %}
      <div class="project-tags">
        {% for tag in project.tags %}<span>{{ tag }}</span>{% endfor %}
      </div>
    {% endif %}
  </section>
{% endfor %}
</div>
