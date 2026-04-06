---
layout: default
---

# Hi, I'm Eyan 👋

I'm a recent Berkeley BSME with experience in manufacturing, robotics, and research. I've worked on many projects, from firefighting robots to next-gen particle accelerators. My engineering approach centers on a first-principles, analytical framework to modularize complex systems. I have a proven track record of managing full-cycle project ownership; from leading the R&D and PLM release of 100+ part assemblies for particle accelerator magnets at LBNL to developing underactuated robotic systems and autonomous fire suppression hardware.

Below, you'll find examples of my previous work. Click the cards to view more!

**I'm looking for work! Recruiter or hiring manager? [Contact me!](mailto:eyan.documet@protonmail.com)**

## 🏢 Work Experience

{% for item in site.data.portfolio.experience %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

## 🛠️ Engineering Projects
Select engineering projects showcasing design, experimentation, and system-level problem solving.

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

## ⛳ Clubs & Organizations

{% for item in site.data.portfolio.clubs %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

## 📰 In the News

{% for item in site.data.portfolio.news %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
