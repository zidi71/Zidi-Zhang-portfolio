---
layout: home
title: "Welcome to My Portfolio"
author_profile: true
classes: wide
---

## 🕒 Posts by Year

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in posts_by_year %}
### {{ year.name }}
<ul>
  {% for post in year.items %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <small>({{ post.date | date: '%b %d' }})</small></li>
  {% endfor %}
</ul>
{% endfor %}

---

## 🗂️ Posts by Category

{% assign categories = "research-oriented,data-oriented,visualizations,psychometrics,sample-data-overview-meeting" | split: "," %}

{% for category in categories %}
### {{ category | capitalize | replace: '-', ' ' }}
<ul>
  {% for post in site.categories[category] %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <small>({{ post.date | date: '%Y-%m-%d' }})</small></li>
  {% endfor %}
</ul>
{% endfor %}
