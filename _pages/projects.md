---
layout: page
title: research
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 1
horizontal: false
---

### Topic 1
<!-- Only show "work" category -->
<div class="projects">
{% assign categorized_projects = site.projects | where: "category", "work" %}
{% assign sorted_projects = categorized_projects | sort: "importance" %}
{% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
{% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
{% endif %}
</div>

---

### Topic 2
<!-- Only show "fun" category -->
<div class="projects">
{% assign categorized_projects = site.projects | where: "category", "fun" %}
{% assign sorted_projects = categorized_projects | sort: "importance" %}
{% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
{% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
{% endif %}
</div>
