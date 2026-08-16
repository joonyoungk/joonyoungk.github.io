---
layout: default
title: "About"
permalink: /
description: "About Joonyoung Kim, an incoming graduate student in transportation engineering at Ajou University."
---

# About

I am a B.S. student in **Transportation System Engineering at Ajou University** and an incoming M.S. student in **Convergence of Data.Network.AI – Transportation Engineering**, beginning in March 2027. I expect to join **[EMI](https://sites.google.com/view/euijinkim)** at Ajou University.

My recent research experience includes demand forecasting for demand-responsive transit, Bayesian modeling and causal analysis, micromobility–public transit interactions, and traffic simulation.

<!--
When your research direction is finalized, uncomment and edit this section.

## Research Interests

- Research interest 1
- Research interest 2
- Research interest 3
-->

## Education

{% include education-list.html %}

## Current Publication

{% assign pub = site.data.publications[0] %}

<div class="featured-publication">
  <h3>{{ pub.title }}</h3>
  <p class="publication-authors">
    {% for author in pub.authors %}
      {% if author.me %}<strong>{{ author.name }}</strong>{% else %}{{ author.name }}{% endif %}{% unless forloop.last %}, {% endunless %}
    {% endfor %}
  </p>
  <p class="publication-venue"><em>{{ pub.venue }}</em>, {{ pub.status }}.</p>
  <a class="inline-link" href="{{ '/publications/' | relative_url }}">View publications →</a>
</div>
