---
layout: default
---

# Hi, I'm Eyan 👋

I'm a mechanical engineer specializing in the design and architecture of complex, first-of-kind multiphysics hardware systems and multi-million-dollar production equipment. 

My background spans advanced research at [UC Berkeley](https://me.berkeley.edu/) and [Lawrence Berkeley National Laboratory](https://www.lbl.gov/), where I engineered precision mechanisms, simulation frameworks, and custom control systems. Today, I architect and deliver mission-critical industrial autoclaves at [ASC Process Systems](https://www.aschome.com).

## Personal Project Portfolio

Artifacts and engineering summaries of recent public-facing work.

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
