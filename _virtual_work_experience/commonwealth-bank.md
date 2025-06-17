---
title: "Commonwealth Bank"
date: 2025-06-10
layout: post
toc:   true
---

---

## Commonwealth Bank

---

Welcome to my Commonwealth Bank Forage work experience recap. Through the Forage virtual simulation, I stepped into the role of a Cybersecurity Generalist on Commonwealth Bank Cybersecurity team, particularly focusing on fraud detection and prevention. This simulation gave me a chance to tackle real-world tasks that help financial institutions keep customer data safe.

During the simulation, I undertook the following tasks:

* Built Splunk dashboards to detect fraud through customer-data pattern analysis.
* Executed cyber-incident response: alerted teams, gathered evidence, contained attacks and supported recovery.
* Designed infographics on secure-password best practices per Australian Cyber Security Centre guidance.
* Conducted web-application penetration tests, identified vulnerabilities and recommended remediation.

Please check out the full report by clicking the link below:

#### **FULL REPORT**
<br>


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