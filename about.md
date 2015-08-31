---
layout: page
title: "Research"
permalink: /about/
---

Publication list at [Google Scholar](https://scholar.google.com/citations?user=8ckkLFgAAAAJ)

We want to be able to predict how populations will evolve.
For example, when a new antibiotic is developed, we need to know
whether it will take bacteria weeks or decades to develop resistance,
and what we can do to affect this.
This goal is just starting to become realistic due to rapid advances in genetic sequencing technology. 
Now we need to solve a pair of theoretical problems in order to translate this sequence data into evolutionary predictions. 
First, we need to understand how to infer prevailing population dynamics from population genomic data 
Second, given these patterns, we need to calculate the spectrum of possible evolutionary trajectories.
Within these broad areas, our research on several key questions listed below.

### Projects:
<ul>
  {% for page in site.html_pages %}
    {% for pc in page.categories %}
      {% if pc == 'project' %}
        <li><a href="{{ page.url }}">{{ page.title }}</a>: {{page.summary}}</li>
      {% endif %}   <!-- cat-match-p -->
    {% endfor %}  <!-- page-category -->
  {% endfor %}  <!-- page -->
</ul>