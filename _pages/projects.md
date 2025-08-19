---
layout: page
title: research
permalink: /projects/
nav: true
nav_order: 1
---

###  Multi-omics Data Analysis

<p align="center">
  <img src="/assets/img/Fig_Omics.png" alt="" width="500">
</p>


Structured dependence is a fundamental characteristic of high-dimensional omics data, arising from complex biological mechanisms such as gene co-expression, protein–protein interactions, and regulatory networks. These dependencies often manifest in block or modular structures that reflect underlying functional units within biological systems. Ignoring such dependence can lead to inflated false discovery rates, biased parameter estimates, and reduced statistical power, ultimately compromising the validity and reproducibility of scientific findings. Developing statistical methods that explicitly account for structured dependence is therefore critical for improving sensitivity, enhancing replicability, and enabling more reliable biological discoveries in omics research.


#### Selected Projects

{% assign work_projects = site.projects | where: "category", "work" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3"
     style="row-gap: 2rem; margin-top: 3rem; margin-bottom: 4rem;">
  {% for project in work_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>

### Neuroimaging Data Analysis


{% assign fun_projects = site.projects | where: "category", "fun" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3"
     style="row-gap: 2rem; margin-bottom: 4rem;">
  {% for project in fun_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>


### Non Euclidan Data Analysis

{% assign fun_projects = site.projects | where: "category", "OODA" | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3" style="row-gap: 2rem;">
  {% for project in fun_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>

