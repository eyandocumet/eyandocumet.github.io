---
layout: default
---

# Hi, I'm Eyan 👋

I am a first-principles mechanical engineer specialized in the development of novel, complex, and coupled hardware systems with a proven history of translating high-level design goals into manufacturable assemblies. I'm experienced across domains of controls, mechatronics, precision systems, multiphysics, and first-of-kind engineering

## Personal Project Portfolio
{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
