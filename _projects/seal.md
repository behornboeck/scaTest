---
layout: post
title: SEAL
feature-img: "assets/img/projects/seal.png"
img: "assets/img/projects/seal.png"
date: 01 September 2017
tags:
---

Side channel attacks use, alongside information such as plaintexts or ciphertexts, leakage about the (secret) key-dependent intermediate state(s), and deliver a  key ranking as a result. Many published works showed that for many practical implementations, observing a few encryptions made complete key recovery possible in practice. The academic research into combating these attacks so far has largely focused on approaches and tools to equip specialised cryptographic engineers with access to a specialist lab and tools.

The research hypothesis of this research project is that one can make meaningful statements about the leakage behaviour of arbitrary implementations on small devices by utilising a-priori derived (instruction level) leakage models. Our vision is to enable developers with limited domain-specific knowledge to perform side channel evaluations at design time without access to a fully equipped lab, by creating tools and methodologies that integrate a priori derived instruction-level leakage models into a standard compiler.

{% include aligner.html images="design.png,LOGO_ERC-FLAG_EU.jpg" %}
