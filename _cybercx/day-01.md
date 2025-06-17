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

On my first day in CyberCX's Cyber5050 Microcredential program, I gained an overview of the Cyber5050 program, and its link to Cyber Accelerator for Women. We also looked at our case study for the next 4 weeks, and as self study, researched the MediSecure ransomware breach.

## What is the Cyber Fundamentals Microcredential?

The Cyber Fundamentals Microcredential is an initiative dedicated to advancing gender equality in cybersecurity. Funded by the Australian Government, it gives 300 women across a 2 year period foundational Cybersecurity knowledge, and offers comprehensive training and leadership development opportunities for women. 

The June-July 2025 cohort is the first group to undertake this training, which I am extremely proud to be part of.

## Goal of the day
The main goal for the first session was to understand how the program fits together and to better understand what the point of Cybersecurity is specifically.

## Tasks Completed
During the lesson, I listened to an overview of the Cyber Accelerator and Cyber5050 programs, which helped me get a better understanding of what the program entails. Then, in the tutorial session, we had a look at the case study we will be looking at the for the next 4 weeks. We looked at a fictitious vocational education provider's IT environment and discussed which components, such as its learning-management system, are most critical.

For homework, I researched the MediSecure ransomware incident from April-June 2024 and drafted a concise case study summarising its impact and the lessons it offers. 

> MediSecure was one of Australia’s main eScript providers, who facilitated the distribution of eScripts and allowed prescribers to send prescriptions to chosen pharmacies across Australia. The company was in operation until late 2023 and ceased trading and entered voluntary administration in June 2024. <br>
>In April 2024, Medisecure became aware of a large-scale ransomware attack which originated from a compromised third-party vendor. In mid-May 2024, the National Cybersecurity Coordinator publicly identified Medisecure as the affected health organisation in Australia's biggest cyber-incident. Details published in July 2024 confirmed that hackers had exfiltrated a database containing names, date of births, addresses, Medicare identifiers and prescription records for up to 12.9million Australians, encompassing prescriptions issued through November 2023. The attackers exfiltrated 6.5TB of data, which contained over 50million rows, and has been sold on the dark web – first for $50,000, then for $25,000. Due to the scale of the incident, Medisecure was not able to pinpoint exactly who was affected by the breach.<br>
> Despite the scale of the breach, prescription services remained uninterrupted due to eRx script exchange running uncompromised. Healthcare providers and patients were advised to be alert of scams, particularly those that reference the MediSecure breach, and be wary of any unsolicited contract purporting to be a medical or financial service provider seeking payment or banking information. The Office of the Australian Information Commissioner (OAIC) launched an inquiry and emphasised that existing privacy legislation was lagging behind evolving cyber threats. <br>
>In June 2024, the company entered voluntary administration due to losing its government contract and the costs related to the breach. <br>
>This incident highlights the need for strong Cybersecurity methods, particularly when handling sensitive data such as health records. There needs to be better data security measures and reforms to privacy laws to better protect personal information in Australia.


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