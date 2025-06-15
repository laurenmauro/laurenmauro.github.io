---
layout: post
title:  "CyberCX Micro‑credential "
permalink: /blog/cybercx/
---

Over the next four weeks I’m writing short daily notes while completing the **CyberCX Fundamentals** credential.  
Select a day below to read the log.

{% assign diary = site.cybercx | sort: "date" %}
<ul>
{% for entry in diary %}
  <li>
    <a href="{{ entry.url }}">{{ entry.title }}</a> –
    {{ entry.date | date: "%-d %b %Y" }}
  </li>
{% endfor %}
</ul>