---
layout: page
title: workshops
permalink: /workshops/
description: De forskellige workshops som jeg faciliterer.
---

{% for workshop in site.workshops %}

{% if workshop.redirect %}

<div class="workshop">
    <div class="thumbnail">
        <a href="{{ workshop.redirect }}" target="_blank">
        {% if workshop.img %}
        <img class="thumbnail" src="{{ workshop.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ workshop.title }}</h1>
            <br/>
            <p>{{ workshop.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="workshop ">
    <div class="thumbnail">
        <a href="{{ workshop.url | prepend: site.baseurl | prepend: site.url }}">
        {% if workshop.img %}
        <img class="thumbnail" src="{{ workshop.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ workshop.title }}</h1>
            <br/>
            <p>{{ workshop.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}
