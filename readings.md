---
layout: post
title: Readings
cover: readings.jpg
permalink: /readings
---

## In-Class Readings

{% assign readings = site.data.papers %}

{% for day in readings %}

### {{ day[0] }}

{% for p in day[1] %}
{% if p.link != None %}
[{{ p.title }}]({{ p.link }}) by {{ p.author }} *{{ p.journal }}* ({{ p.year }}). {{ p.description }}
{% elsif p.PDF != None %}
[{{ p.title }}]({{ site.baseurl }}/papers/{{ p.PDF }}) by {{ p.author }} *{{ p.journal }}* ({{ p.year }}). {{ p.description }}
{% else %}
{{p.title}} by {{ p.author }} *{{ p.journal }}* ({{ p.year }}). {{ p.description }}
{% endif %}
{% endfor %}
{% endfor %}



## external resources
Links to external databases and other resources that you may find helpful during the course.

* [Physical Biology of the Cell (online pandemic version)](https://www.youtube.com/@physicalbiologyofthecellca307/). This YouTube channel is home to hundreds of vignettes which Rob recorded for the remote version of this course; you may enjoy revisiting concepts we've covered in person this week at your own pace.

* [The Bionumbers Database](https://bionumbers.hms.harvard.edu/search.aspx). An incredibly handy collection of numbers from the molecular and cell biology literature.

* [The Human Impacts Database](https://anthroponumbers.org/). Useful quantities describing the interactions of humans with Earth's land, oceans, atmosphere, flora and fauna.

* [Street-Fighting Mathematics: The Art of Educated Guessing and Opportunistic Problem Solving](https://sept.mit.edu/sites/default/files/Streetfighting%20Mathematics.pdf). This excellent free book by Sanjoy Mahajan (a Caltech alum!) teaches order-of-magnitude estimation in the same style that we will employ throughout the course. Essential reading for those curious to explore more advanced techniques than those we will cover.
