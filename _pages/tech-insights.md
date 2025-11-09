---
title: "Tech Insights"
permalink: /tech-insights/
---

Notes on tools, code patterns, and design decisions from my PhD projects.

### Selected Topics
- Build systems (CMakePresets, vcpkg manifest)
- C++ / Rust interop
- Simulation middleware (ROS 2, PX4, ZeroMQ)
- Parameter schema design

---

**Latest posts**

{% for post in site.posts limit:10 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%b %d, %Y" }}
{% endfor %}
