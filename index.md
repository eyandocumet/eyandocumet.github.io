---
layout: default
---

# Hi, I'm Eyan 👋

I'm a Berkeley grad specialized in mechatronics and R&D. From integrating next-gen particle accelerator assemblies to developing underactuated robotic systems, I thrive on high-stakes engineering challenges where precision and project ownership are non-negotiable.

**I'm looking for work! Recruiter or hiring manager? [Contact me!](mailto:eyan.documet@protonmail.com)**

Below, you'll find examples of my previous work. Click the cards to view more!

## 🏢 Professional Experience

{% for item in site.data.portfolio.experience %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

## 🛠️ Portfolio Projects

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
