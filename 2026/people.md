---
layout: 2026_post
title: People
permalink: /2026/people
---

# V. People


{% for author in site.data.2026.members %}
<div id="im">
    <figure>
        {% if author.link %}
        <b> <a href="{{ author.link }}">{{ author.name }}</a></b><br>
        {% else %}
        <b> {{ author.name }} </b><br>
        {% endif %}
        <img src="{{ site.baseurl }}/2025/assets/images/people/{{ author.image }}" width="200" height="200"><br>
        {{ author.role }}<br>
        <figcaption>
        <code>{{ author.email }}</code>
        </figcaption>
    </figure>
</div>
{% endfor %}
