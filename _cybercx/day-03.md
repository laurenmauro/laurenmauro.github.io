---
title: "Day 03 - Threat Actors, MITRE ATT&CK and Social Engineering"
date: 2025-06-18
layout: post
toc:   true
---

---

**Table of Contents**
1. TOC  
{:toc}

---

On day three of the CyberCX Cyber5050 microcredential, we looked at different types of threat actors, particularly their skill levels and what motivates them, and how to apply this understanding to defend against attacks. We also had a look at the Cyber Kill Chain and ended by looking at Social Engineering attacks and how AI is worsening the effects of it.


## Goal of the day
The goal for today was to understand common threat actors and to work out their skills and motivations, as well as learning the frameworks such as the Cyber Kill Chain and MITRE ATT&CK, which will help us expose the steps adversaries take so we can intervene earlier.

## Tasks Completed

Firstly, we listened to a lecture on threat actors. Particularly, we learnt what they are, their skill levels on a tier basis (1-6, with 6 being most skilled) and the different threat actor groups and their motivations. We also differentiated between opportunistic and targeted attacks and considered the different types of cyber attacks. One thing that was a new concept to me was the idea of "attribution" - are we sure that this is the adversary that perpetuated this cyber attack? 

We also had a look at MITRE and the ATT&CK Kill Chain. This is something I've heard of but haven't really dived deep into. The MITRE ATT&CK kill chain was quite intimidating and long, with lots of techniques for various types of behaviour like lateral movement, initial access and execution. Then we looked at the Cyber Kill Chain from Lockheed Martin which was for more digestable and comprised of 7 stages: reconnaissance, weaponisation, delivery, exploitation, installation, command and control and actions and objective. Later we had to apply this to the Medisecure breach.

Finally, we briefly looked at social engineering, particularly the common tactics used and how AI has been used to worsen the scale and impact of social engineering attacks.

## Key Learnings

One thing I found interesting was a brief story about how reconnaissance can go beyond the keyboard and be physical, like imitating staff to gain access to businesses. This was quite shocking because it shows how easily human trust and assumptions can be exploited in the physical world. It brings me back to the idea we learnt yesterday about People, Processes and Technology; even if our processes and technology are strong within the business, people are often the weakest link and their negligence leads to vulnerabilities.

## Personal Reflection

I've realised how important it is for the "People" component of the PPT triad to be cyber-aware to avoid unintentional access to adversaries. Now, I want to polish up on what I learnt today, particularly the types of threat modelling and kill chains, to improve my knowledge.

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