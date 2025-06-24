---
title: "Day 05 - Presentations 101"
date: 2025-06-20
layout: post
toc:   true
---

---

**Table of Contents**
1. TOC  
{:toc}

---

On day five of the Cyber5050 microcredential, we focused on Presentation 101. We learned how to create slides that engage non-technical viewers and then applied those principles by creating a three-page briefing on the MediSecure breach.

## Goal of the day
The goal for today was to master the slide structure and language for an audience that is non-technical, such as CEOs and CFOs. It was also to understand the essentials of presentations such as grabbing attention, conveying key messages simply and leaving a lasting impression.

## Tasks Completed

We covered best practices for opening with a quote, fact or story. We then learnt that we must be structuring slides around one main idea, choosing goals (inform, persuade, inspire) and supporting points with examples, stories and visuals. We also learned to manage timing, leave space for questions, and adding a personal style, which we learnt are skills we will cultivate as we advance in our career. Finally, we applied all these principles to create a three-slide executive briefing on the 2024 MediSecure breach overview

## Key Learnings

I learnt that less really is more. I was able to create a three-side briefing with minimal text and clear graphics to communicate to my audience well. I also learnt that it's important to tailor language and examples to non-technical users like CFOs and CEOs is important. For example, instead of saying "the ransomware will lead to a breach of confidentiality for the company," it can be replaced with "the attack led to credentials being stolen and a $30 million loss of revenue for the company."

## Personal Reflection

I have realised that it is important to communicate in a purposeful way to non-technical viewers, which can be difficult. This makes me realise that soft skills are quite important in Cybersecurity and people often don't put much of an emphasis on their importance. For my next slideshow, I will reduce the amount of text on the screen and communicate with dot-points and visuals instead.

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