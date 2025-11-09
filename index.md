---
layout: home
title: "Engineering Notes & Research"
author_profile: false
sidebar:
  nav: "main"
---

Welcome! This is my collection of research notes, technical documentation, and
programming insights from my PhD in robotics and control systems.

The site is divided into three parts:

- 🧑‍🔬 [**About Me / CV**](/about/) — background and academic record
- 📚 [**Research**](/research/) — summaries of key research directions
- ⚙️ [**Tech Insights**](/tech-insights/) — engineering notes and code
  deep-dives

---

### 🆕 Recent Posts

{% for post in site.posts limit:5 %}

- [{{ post.title }}]({{ post.url | relative_url }}) —
  {{ post.date | date: "%b %d, %Y" }} {% endfor %}
