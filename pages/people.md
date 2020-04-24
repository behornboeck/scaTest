---
layout: page
title : People
permalink: /people/
subtitle: "Current Team Members"
feature-img:
tags:
---


<ul>
{% for member in site.data.staff %}
  <li>
    <a href="{{ member.url }}">
      {{ member.name }},
    </a> {{ member.position }}
  </li>
{% endfor %}
</ul>


Past staff members of Elisabeth's team:
<ul>
{% for member in site.data.paststaff %}
  <li>
    <a href="{{ member.url }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>
