---
layout: home
title: "Welcome to My Portfolio"
author_profile: true
classes: wide
---

## 💡 What I Value

<span style="font-size: 1.1rem; line-height: 2;">
Researching for equity.<br>
Measuring for meaning.<br>
Writing for inclusion.<br>
Visualizing for clarity.<br>
Evaluating for growth.
</span>

---

## 🗂️ Project Categories

{% assign categories = "Policy Research,Data-analysis,visualizations,psychometrics,Sample Data-overview Meeting" | split: "," %}

{% for category in categories %}
### {{ category | replace: '-', ' ' | capitalize }}
<ul>
  {% for post in site.categories[category] %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <small>({{ post.date | date: '%Y-%m-%d' }})</small></li>
  {% endfor %}
</ul>
{% endfor %}
