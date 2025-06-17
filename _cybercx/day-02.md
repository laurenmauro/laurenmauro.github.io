---
title: "Day 02 - CIA and Frameworks"
date: 2025-06-17
layout: post
toc:   true
---

---

**Table of Contents**
1. TOC  
{:toc}

---

On day two of the CyberCX Cyber5050 microcredential, we focused on the CIA triad and how to apply it to to IT environments - particularly our case study. We also reviewed various cybersecurity frameworks and practiced mapping both the triad and frameworks to the ES Learning case study.


## Goal of the day
The goal for today was to understand the three pillars of the CIA triad, and learn how to implement control, program and risk frameworks to protect IT and OT systems.

## Tasks Completed

First, we listened to a lecture on the CIA triad definitions and how, in specific Cyber incidents, that facet of the CIA triad was compromised. We also discussed why OT systems like industrial controllers and sensors must also be included along IT systems when assessing CIA. We also looked at some ways the parts of CIA triad can be implemented. 

We also learnt the three categories of frameworks used in Cybersecurity -
* Control frameworks like NIST 800-53, CIS Controls and ASD Essential Eight
* Program frameworks such as ISO 27001 and NIST CSF
* And finally, Risk frameworks like NIST 800-39, ISO 27005 and FAIR.

Furthemore, we explored the idea of Defence in Depth, which is a cybersecurity strategy that uses multiple layers of security for holistic protection. We also differed Defense in Depth to Layered Security - even though they are used interchangeably, defense in depth is a broader, more strategic approach, but layered security is a specific component of that strategy, focusing on multiple layers.

## Key Learnings

One thing I found particularly interesting was that OT systems are now targetable and must be protected under the same CIA principles. Ignoring OT can expose critical physical processes to risks. At uni, we were only taught to implement them in IT scenarios, not OT - so I found this extremely interesting.

Another thing that was interesting was that Cybersecurity frameworks aren't a stock-standard solution or best practice, but rather a starting point. Since I want to get into GRC, this is something I will need to keep in mind.

## Personal Reflection

When looking at cyber incidents now, instead of just assuming data-centric risks only affect servers, I will start by listing critical capabilities across both IT and OT. Mapping CIA for each system in our case study helped me see how these controls align with service goals.

I also want to try mapping difference frameworks to another case study / fictional business to improve my understanding of different frameworks.

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