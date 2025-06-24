---
title: "Day 07 - Cryptography"
date: 2025-06-23
layout: post
toc:   true
---

---

**Table of Contents**
1. TOC  
{:toc}

---

On day seven of the Cyber5050 microcredential, we looked at Cryptography, particularly its key concepts, classic ciphers used and the real-world uses. We reviewed how encryption and hashing protect data and explored methods like steganography and PKI before doing a hands-on cipher challenge independently.


## Goal of the day
The aim was to understand cryptography's purposes - hiding messages, verifying senders and ensuring data integrity. We aimed to understand the difference between symmetric and asymmetric algorithms, as well as hashing, and how they can be applied to modern security systems.

## Tasks Completed

We began by looking at key terminology and the history of Cryptography. It was quite interesting to learn that cryptography goes back to the Ancient Greece days, and it's clever how they were able to encrypt information back then. Then, we learnt about different algorithms. Firstly, we looked at symmetric algorithms, including DES, 3DES and AES. We learnt that DES was able to be cracked back in 1998 and that AES is the best symmetric algorithm to use in modern contexts.  Then we looked at public-key cryptography, which compared to symmetric, uses two pair of keys - the public and private, to make it more secure. Then we looked at hashing algorithms such as SHA-1, SHA-2 and SHA-3 which are used to obscure important information and cannot be reversed.

We then looked at how this is used in the real world. We looked firstly at steganography, which was quite cool but difficult to wrap my head around - how can a seemingly normal picture hold hidden information? Then we explored digital signatures in Public Key Infrastructures, SSL/TLS handshakes and S/MIME for email.

Although I have just completed a subject on Cryptography at uni this semester, it was interesting to see real-world applications and focus on the less mathematical part of crypto.

## Key Learnings

We had to complete a cipher challenge for our homework. It blended several methods - decimal decoding, braille to words, ROT-13 and columnar transposition ciphers, as well as steganography of a .WAV file, which had a hidden message within the graph. It was challenging but extremely fun to work through and was a nice activity to understand how Cryptography can be used in the real world.

## Personal Reflection

I was really proud to have solved the entire puzzle end-to-end and on my own. Since I found the coursework in my uni Cryptography class a bit challenging, it was nice to have it reinforced and explained in this course. I would love to do some more of those decoding challenges as a fun puzzle!

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