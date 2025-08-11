---
title: Projects
nav:
  order: 2
  tooltip: Software, datasets, and more
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects

Our projects span various domains of AI and machine learning, from developing novel speculative decoding systems for efficient LLM inference to creating innovative solutions for distributed computing and edge AI. Each project combines rigorous research with practical applications, addressing real-world challenges in modern AI systems.

Below you'll find our featured projects and ongoing research initiatives that demonstrate our commitment to advancing the state-of-the-art in intelligent systems.

{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}

{% include section.html %}

## Featured

{% include list.html component="card" data="projects" filter="group == 'featured'" %}

{% include section.html %}

## More

{% include list.html component="card" data="projects" filter="!group" style="small" %}
