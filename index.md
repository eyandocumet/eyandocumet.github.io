---
layout: default
---

# Hi, I'm Eyan 👋

Here's some of my previous work:

{% for item in site.data.portfolio.jobs %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
