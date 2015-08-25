---
layout: page
title: "Research"
permalink: /about/
---

Publication list at [Google Scholar](https://scholar.google.com/citations?user=8ckkLFgAAAAJ)

I build and analyze models of biological populations to predict their future evolution. 
Ultimately, we would like to understand evolution well enough that, for example, when a new antibiotic is developed, 
a reasonable number of experiments would be enough to learn how long it would take for bacteria to become resistant. 
This goal is just starting to become realistic due to rapid advances in sequencing technology. 
Now we need to solve a pair of theoretical problems in order to translate this sequence data into evolutionary predictions. 
First, we need to understand how to infer prevailing population dynamics from population genomic data — given a set of sequenced individuals, what can we learn about patterns of reproduction, migration, and adaptation in the population that they came from? 
Second, given these patterns, what do we expect the population to do in the future, and how can we test our predictions in scaled-down lab populations? 
A particular focus of my work on this second problem has been on understanding the likelihood and dynamics of complex adaptations whose benefits require combinations of multiple mutations.

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