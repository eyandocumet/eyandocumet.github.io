---
layout: default
---

# Hi, I'm Eyan 👋

I'm a **Mechanical Engineer** from **UC Berkeley** focused on **testing**, **simulation**, and **electromechanical design**. I've previously worked at [LBNL](lbl.gov) as a Mechanical Engineering R&D Intern. Below, you'll find the technical documentation and results of my engineering projects.

**Recruiter or hiring manager? [Contact me!](mailto:eyan.documet@protonmail.com)**

{% for item in site.data.portfolio.jobs %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
