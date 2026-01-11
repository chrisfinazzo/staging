---
layout: page
title: Links
permalink: /links/
---

{% assign linksByDay = site.links | group_by_exp: "link", "link.date | date: '%A, %B %d, %Y'" %}

{% for day in linksByDay reversed %}
<h2>{{ day.name }}</h2>
{% for link in day.items reversed %}
<h3><a href="{{ link.url }}">{{ link.title }}</a></h3>
{{ link.content }}
{% endfor %}
{% endfor %}
