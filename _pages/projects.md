---
layout: page
title: research
permalink: /projects/
nav: true
nav_order: 1
---

### Topic 1
{% assign work_projects = site.projects | where: "category", "work" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3">
  {% for project in work_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>

### Topic 2
{% assign fun_projects = site.projects | where: "category", "fun" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3">
  {% for project in fun_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>
