---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
nav_order: 1
---

For the latest updates, please visit my [Google Scholar](https://scholar.google.com/citations?user=RD1KjEkAAAAJ).
<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}
 
<div class="publications">
<h2><span>Statistical Methodology</span></h2>
 
{% bibliography --query @*[category=method] %}
 
<h2><span>Applications</span></h2>
 
{% bibliography --query @*[category=application] %}
 
</div>
