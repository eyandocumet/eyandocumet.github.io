---
layout: default
---

# Hi, I'm Eyan 👋

I'm a mechanical engineer specializing in the design, development, and execution of novel and/or complex multiphysics hardware systems. I've contributed to efforts at [UC Berkeley](https://www.berkeley.edu/) and [Lawrence Berkeley National Laboratory](https://www.lbl.gov/), developing first-of-kind precision mechanisms, simulation tools, and control systems.

Currently, I design and deliver specialized, multi-million-dollar autoclave and process systems at [ASC](aschome.com). My experience spans mechatronics, precision motion, and complex mechanical assemblies, with a focus on turning early-stage concepts into reliable, manufacturable hardware.

## Personal Project Portfolio
{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
