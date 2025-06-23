---
title: "Day 04 - Risk Management and Privacy"
date: 2025-06-19
layout: post
toc:   true
---

---

**Table of Contents**
1. TOC  
{:toc}

---

On day six of Cyber5050, we focused on how data moves through an organisation and how to keep it safe. We covered data classifications, backup and recovery methods, and tools for preventing unauthorised data loss. We finished with an overview of secure data destruction and data-loss prevention solutions.


## Goal of the day
The aim was to learn how to identify different data types and their sensitivity levels, understand best practices for backups and resilience, and explore methods for stopping data leakage and securely disposing of records. 

## Tasks Completed

We began by classifying data into categories such as public, confidential, critical and personal. Next, we covered how data exists at rest, in transit and in use, and reviewed the roles responsible for managing it. We then looked at back-up types - full, incramental and differential, and for our workbook task, practiced designing a backup strategy for MediSecure. We also compared backups to redundancy solutions like RAID, and discussed why RAID alone can’t replace a proper backup. Finally, we looked at data-loss prevention (DLP) tools and reviewed secure destruction methods for both hard disks and encrypted data.

## Key Learnings

I was surprised to learn that many organisations never test their backups and simply assume they will work when needed. Without regular restore drills, backups may fail unnoticed. Therefore, all companies should adopt good backup practice, meaning scheduling restores and verifying each step.

{% comment %}
  Compute current, previous, and next day numbers
{% endcomment %}
{% assign today = page.slug | remove: "day-" | plus: 0 %}
{% assign prev  = today | minus: 1 %}
{% assign next  = today | plus: 1 %}
{% assign total = site.cybercx | size %}

<nav class="day-nav">
  {% if prev >= 1 %}
    {% assign prev_str = prev | prepend: "0" | slice: -2, 2 %}
    <a href="/cybercx/day-{{ prev_str }}/">« Previous Day</a>
  {% endif %}

  {% if prev >= 1 and next <= total %}
    &ensp;|&ensp;
  {% endif %}

  {% if next <= total %}
    {% assign next_str = next | prepend: "0" | slice: -2, 2 %}
    <a href="/cybercx/day-{{ next_str }}/">Next Page »</a>
  {% endif %}
</nav>