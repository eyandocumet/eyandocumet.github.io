---
layout: default
---

# Hi, I'm Eyan 👋

I'm a **Mechanical Engineer** from **UC Berkeley** focused on **testing**, **simulation**, and **electromechanical design**. Below, you'll find examples of my previous work.
**I'm looking for work! Recruiter or hiring manager? [Contact me!](mailto:eyan.documet@protonmail.com)**

## Portfolio
Below are some artifacts from work I've done in the past. Click the cards to learn more!

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
