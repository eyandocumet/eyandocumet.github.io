---
layout: default
---

# Hi, I'm Eyan 👋

I'm a Mechanical Engineer obsessed with solving high-stakes, highly-technical problems. I'm specialized in advanced manufacturing, process systems, and designing around multi-physical constraints.

My background includes leading hardware R&D for a particle accelerator prototype at LBNL, as well as various mechatronics and simulation projects at UC Berkeley. Currently, I'm lending my skills to designing autoclaves and process systems at ASC. I focus on creating clean, highly readable designs and moving complex projects securely through the release process.

Below are some of my previous independant or school-related work:

{% for item in site.data.portfolio.jobs %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
