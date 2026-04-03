---
layout: default
---

# Hi, I'm Eyan 👋

I'm a recent Berkeley BSME with experience in manufacturing, robotics, and research. I've worked on many projects, from firefighting robots to next-gen particle accelerators. Project ownership is important to me, so I enjoy involvement in as many parts of the process as possible. My ideal workday balances time designing and analyzing with time on the shop floor. I work well with others and have led many projects during my time at UC Berkeley and the Lab. I pride myself on my ability to make engineering decisions under pressure.

The more complex a problem is, the more excited I am to solve it. I'm especially interested in anything high-tech: robotics, aerospace, advanced manufacturing, green energy. If you agree with my philosophy, let's connect!

Below, you'll find examples of my previous work. Click the cards to view more!

**I'm looking for work! Recruiter or hiring manager? [Contact me!](mailto:eyan.documet@protonmail.com)**

## 🏢 Work Experience
Hands-on engineering roles and teaching experiences demonstrating technical proficiency and leadership.

{% for item in site.data.portfolio.experience %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

## 🛠️ Engineering Projects
Select engineering projects showcasing design, experimentation, and system-level problem solving.

{% for item in site.data.portfolio.projects %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

## ⛳ Clubs & Organizations
Extracurricular leadership and team-based engineering experiences

{% for item in site.data.portfolio.clubs %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}

## 📰 In the News
Notable public outreach and leadership highlights.

{% for item in site.data.portfolio.news %}
  {% include card.html title=item.title description=item.description image=item.image url=item.url tags=item.tags %}
{% endfor %}
