---
layout: post
title: Virtual Work Experience
description: View my Forage virtual work experience write-ups
permalink: /projects/virtual-work-experience/
---

Welcome to my Virtual Work Experience page. Here you will find the Cybersecurity programs I have completed through Forage. Forage is an online platform offering self-paced virtual work experience programs that simulate the tasks and scenarios professionals encounter in the cybersecurity field.

On this page you will find links to each Cybersecurity program I undertook, where you can read my write-ups in more detail. Each has the objectives I worked towards, the challenges address and techniques applied to develop solutions.

Feel free to explore each module to see how I've built practical Cybersecurity skills through these experiences!

<ul>
{% assign diary = site.virtual_work_experience | sort: "date" %}
{% for entry in diary %}
  <li>
    <a href="{{ entry.url }}">{{ entry.title }}</a> –
    {{ entry.date | date: "%-d %b %Y" }}
  </li>
{% endfor %}
</ul>
