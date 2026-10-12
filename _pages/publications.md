---
layout: page
permalink: /publications/
title: Publications
description: Papers, preprints, and talks in reverse chronological order.
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->
<!-- Add entries to _bibliography/papers.bib; they are rendered automatically by jekyll-scholar. -->

{% capture pub_count %}{% bibliography_count %}{% endcapture %}

{% if pub_count == "0" %}

<p class="publications-empty">Nothing listed yet — papers and talks will appear here as they come out.</p>

{% else %}

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

{% endif %}
