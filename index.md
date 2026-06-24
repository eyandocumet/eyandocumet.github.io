---
layout: default
---

# Hi, I'm Eyan 👋

I am a Mechanical Engineer driven by solving high-stakes, multi-physical engineering challenges. I specialize in advanced manufacturing, mechatronics, and designing hardware under tight thermal and structural constraints.

Currently, I design and execute massive industrial autoclaves and complex process systems at ASC Process Systems, focusing on systems-level engineering and project management. Previously, I led mechanical hardware R&D for a particle accelerator prototype at Lawrence Berkeley National Laboratory and developed custom multiphysics simulation tools and robotics at UC Berkeley.

## Work Experience
{% for item in site.data.portfolio.jobs %}
  {% include card.html title=item.title description=item.description url=item.url tags=item.tags %}
{% endfor %}

## School Experience
{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
