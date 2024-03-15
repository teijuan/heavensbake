---
layout: page
title: "Clips"
permalink: /clips/
---

  <ul>
    {% assign sorted = site.clips | sort: 'date' | reverse %}
    {% for item in sorted %}
      <a href="{{ item.url }}">
        <img class="filmCover" src="{{ site.url }}/assets/img/clips/{{ item.slug }}.jpg" alt="{{ item.slug }}">
      </a>
    {% endfor %}
  </ul>
  
