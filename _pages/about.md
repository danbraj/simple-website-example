---
layout: page
permalink: /about
title: About
---

## About me

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vitae odio non ligula molestie sagittis. Praesent sed ultricies tortor. Aenean malesuada sodales imperdiet. Duis justo velit, ornare id posuere in, pulvinar ac sapien. In sed sapien eget magna vestibulum congue nec vitae sem. Duis commodo posuere nibh et dignissim. Nulla bibendum auctor nisl at malesuada.

{% if site.data.likes %}
<h2>What I like</h2>
<ul class="likes">
    {% for like in site.data.likes %}
    <li class="like">
        <a class="like__link" href="{{ like.link }}">
            {% if like.image %}
            <img class="like__image" src="{{ like.image }}" alt="">
            {% endif %}
            <span class="like__name">{{ like.name }}</span>
        </a>
    </li>
    {% endfor %}
</ul>
{% endif %}