---
title: "Day 01 – Orientation"
date: 2025-06-15
layout: post
toc:   true
---

---

**Table of Contents**
1. TOC  
{:toc}

---

## Goal of the day

## Tasks Completed

## Key Learnings

## Challenges and Solutions

## Personal Reflection


{% comment %}
  Compute current day number and the next one
{% endcomment %}
{% assign today = page.slug | remove: "day-" | plus: 0 %}
{% assign next  = today | plus: 1 %}
{% assign total = site.cybercx | size %}

{% if next <= total %}
  {% comment %}
    Pad “3” → “03”, “12” → “12” by prepending “0” then taking last 2 chars
  {% endcomment %}
  {% assign next_str = next | prepend: "0" | slice: -2, 2 %}

  <nav class="next-day-nav">
    <a href="/cybercx/day-{{ next_str }}/">
      Next Day »  
    </a>
  </nav>
{% endif %}