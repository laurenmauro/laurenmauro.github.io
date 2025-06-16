---
title: "Day 01 – Introduction"
date: 2025-06-16
layout: post
toc:   true
---

---

**Table of Contents**
1. TOC  
{:toc}

---

On my first day in CyberCX's Cyber5050 Microcredential program, I gained an overview of the Cyber5050 program, its link to Cyber Accelerator for Women. We also looked at our case study for the next 4 weeks, and as self study, researched the MediSecure ransomware breach.

## What is the Cyber Fundamentals Microcredential?

The Cyber Fundamentals Microcredential is an initiative dedicated to advancing gender equality in cybersecurity. Funded by the Australian Government, it gives 300 women across a 2 year period foundational Cybersecurity knowledge, and offers comprehensive training and leadership development opportunities for women. 

The June-July 2025 cohort is the first group to undertake this training, which I am extremely proud to be part of.

## Goal of the day
The main goal for the first session was to understand how the program fits together and to better understand what the point of Cybersecurity is specifically.

## Tasks Completed
During the lesson, I listened to an overview of the Cyber Accelerator and Cyber5050 programs, which helped me get a better understanding of what the program entails. Then, in the tutorial session, we had a look at the case study we will be looking at the for the next 4 weeks. We looked at a fictitious vocational education provider's IT environment and discussed which components, such as its learning-management system, are most critical.

For homework, I researched the MediSecure ransomware incident from April-June 2024 and drafted a concise case study summarising its impact and the lessons it offers. 

## Key Learnings

One thing I found particularly interesting was the idea that effective cybersecurity begins with knowing what you are protecting, and that we are "protecting a capability not just a network." Framing security around the capability to deliver services shifts the focus onto maintaining functionality and trust. 


## Personal Reflection

When looking at cyber incidents now, I will make sure to look at it through this lens, particularly considering which capability needs to be protected within a business. It showed me that I need to start any security plan by listing the services and functions that must stay online, rather than by focusing on individual devices.

I plan to use this approach in my next vulnerability management exercise, mapping each control back to the specific capability it protects.


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