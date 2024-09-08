---
layout: page
title: "Fanmade Media"
permalink: /fanmade/
excerpt: "Fan-made works of our characters"
---

**Fan-made artworks and other content casting our characters**

<ul>
{% for item in site.data.fanmade %}
    {% if item.url %}
        <a href="{{ item.url }}"><img src="/assets/icons/fanmade/{{ item.source }}" style="width: 128px" alt="{{ item.alt }}   "></a>
    {% else %}
        <img src="/assets/icons/fanmade/{{ item.source }}" style="width: 128px" alt="{{ item.alt }}">
    {% endif %}

{% endfor %}
</ul>
