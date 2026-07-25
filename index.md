---
layout: default
---

# Hi, I'm Eyan 👋

I'm a mechanical engineer who designs and builds novel multiphysics hardware systems. 
I have direct experience in first-of-kind precision mechanisms and multi-million-dollar production equipment.

Previously, I contributed to research at [UC Berkeley](https://me.berkeley.edu/) and 
[Lawrence Berkeley National Laboratory](https://www.lbl.gov/), developing precision 
mechanisms, simulation tools, and control systems. Today, I design and deliver 
specialized industrial autoclaves at [ASC Process Systems](https://www.aschome.com).

**Core areas:** Mechatronics · Precision Motion · Multiphysics Simulation · Control Systems · DFx

## Personal Project Portfolio

Artifacts and summaries of recent public-facing work.

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
