---
layout: post
title: people
cover: phage.jpg
permalink: /people
---

{% for author in site.data.members %}
{% if author.role == 'instructor' %}
<div id="im">
<figure>
<b> <a href="{{ author.link }}">{{ author.name }}</a></b><br>
<img width='200' height='200' src="{{ site.baseurl }}/assets/images/people/{{ author.image }}"><br>
{{ author.role }}<br>
<!-- ({{ author.pronouns }})<br> -->
<figcaption>
<code>{{ author.email }}</code>
</figcaption>
</figure>
</div>
{% endif %}
{% endfor %}


{% for author in site.data.members %}
{% if author.role != 'instructor' %}
<div id="im">
<figure>
{% if author.link %}
<b> <a href="{{ author.link }}">{{ author.name }}</a></b><br>
{% else %}
<b> {{ author.name }} </b><br>
{% endif %}
<img src="{{ site.baseurl }}/assets/images/people/{{ author.image }}" width="200" height="200"><br>
{{ author.role }}<br>
<figcaption>
<!-- ({{ author.pronouns }})<br> -->
<code>{{ author.email }}</code>
</figcaption>
</figure>
</div>
{% endif %}
{% endfor %}
