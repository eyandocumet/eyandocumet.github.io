---
layout: default
---

# Hi, I'm Eyan 👋

I'm a Mechanical Engineer obsessed with solving high-stakes, highly-technical problems. I'm specialized in advanced manufacturing, electromechanical systems, and designing around multi-physical constraints.

Currently, I'm lending my skills to designing autoclaves and process systems at ASC. My background includes leading hardware R&D for a particle accelerator prototype at LBNL, mechatronics and simulation projects at UC Berkeley.

## Work Experience
{% for item in site.data.portfolio.jobs %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}

## School Experience
{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
