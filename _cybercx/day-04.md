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

On day four of the Cyber5050 program, we moved from understanding attackers and what they do, to how we defend. We looked at risk management and defined what a risk is, and what privacy is in the cyber space.


## Goal of the day
The goal for today was to understand risk concepts, particularly the difference between threats and vulnerabilities, what makes inheret, current and residual risks unique, and how to undertake risk management. We also set out to consider the requirements surrounding privacy issues in cyber security.

## Tasks Completed

Firstly, we started by defining risk under ISO 31000 standards and what effective risk management entails, including minimising organisation's likelihood's of security incidents and improving their security posture. We also looked at risk appetite vs tolerance - where risk appeitite is what an organisation is willing to accept on an everyday basis, whilst risk tolerance is what an organisation is willing to accept above its risk appetite. Furthermore, we also defined the different stages of risks (inherent, current and residual) and what makes them different.

We then looked at risk management techniques, such as quantitative and qualitative analysis. We defined the risk equation and had a look at the qualitative/semi-qualitative risk assessment heat maps and applied it to an example. Then, we looked at Quantitative risk analysis briefly - although we were told we don't use this in cyber.

Later, we covered privacy and what it is. We covered what personal information is and how it differs to personal identifiable information. Furthermore, we looked at the intersection of privacy and security, and what makes them the same and different. 

## Key Learnings

One thing I found interesting was the myth busting discussion on whether apps like Alexa, Siri or Facebook are actually listening to us all the time. Even though there's plenty of fear-mongering, we found out that these platforms don't record all conversations, unless there is some form of user consent through the Terms of Service or app permissions. As a fun experiment, we were told to say "trampoline" three times and check if we get any trampoline related ads by the end of the course (I probably won't but I'll keep an eye out just in case).

I also found it interesting that risk management isn't about eliminating *all* risk, but making informed decisions. Knowing when to accept, transfer or reduce risk is driven by cost, impact and risk appetite. I also found the idea of risk appetite and risk tolerance interesting.

## Personal Reflection

I've realised that there is a lot of fear-mongering on the internet and a lot of the "my phone is listening to me!!" anecdotes are more than likely just coincidence or sites/apps tracking your search data for targeted advertising. I have also realised I need to be more careful online shopping - I do put a lot of precautions into place (eg. only using Apple Pay, using a fake email) but I must do more to keep my personal information safe, because companies don't care about your privacy and just want money!

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