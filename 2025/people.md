---
layout: 2025_post
title: People
permalink: /2025/people
---

# V. People


{% for author in site.data.members %}
<div id="im">
    <figure>
        {% if author.link %}
        <b> <a href="{{ author.link }}">{{ author.name }}</a></b><br>
        {% else %}
        <b> {{ author.name }} </b><br>
        {% endif %}
        <img src="{{ site.baseurl }}/assets/images/people/{{ author.image }}" width="200" height="200"><br>
        {{ author.role }} ({{ author.pronouns }})<br>
        <figcaption>
        <code>{{ author.email }}</code>
        </figcaption>
    </figure>
</div>
{% endfor %}
