---
layout: page
title: research
permalink: /projects/
nav: true
nav_order: 1
---

###  Multi-omics Data Analysis


{% assign work_projects = site.projects | where: "category", "work" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3" style="row-gap: 2rem;">
  {% for project in work_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>

### Neuroimaging Data Analysis


{% assign fun_projects = site.projects | where: "category", "fun" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3" style="row-gap: 2rem;">
  {% for project in fun_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>
