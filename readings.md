---
layout: post
title: Readings
---

# IV. Readings

Throughout the course, we will frequently encounter relevant literature, new and old.
Although we won't have time to discuss all of it in detail, we'll post links to these readings here for your own perusal.
(If you find something interesting that we haven't listed here, let us know!)

{% assign readings = site.data.papers %}

{% for day in readings %}

### {{ day[0] }}

{% for p in day[1] %}
{% if p.link != None %}
* [{{ p.title }}]({{ p.link }}) by {{ p.author }} *{{ p.journal }}* ({{ p.year }}). {{ p.description }}
{% elsif p.PDF != None %}
* [{{ p.title }}]({{ site.baseurl }}/papers/{{ p.PDF }}) by {{ p.author }} *{{ p.journal }}* ({{ p.year }}). {{ p.description }}
{% else %}
* {{p.title}} by {{ p.author }} *{{ p.journal }}* ({{ p.year }}). {{ p.description }}
{% endif %}
{% endfor %}
{% endfor %}

## Preliminary reading

In December, we suggested several books in advance of this course.
All of them come highly recommended, and in at least one case, you will even have the chance to meet the author.

* [How to Speak Whale](https://books.google.com/books/about/How_to_Speak_Whale.html?id=ArNXEAAAQBAJ), by Tom Mustill. How modern science and machine learning are being used to study cetacean communication.

* [At the Water's Edge](https://books.google.com/books/about/At_the_Water_s_Edge.html?id=fxHrAwAAQBAJ), by Carl Zimmer. A history of two important evolutionary transitions: fins to limbs (our Devonian ancestors arriving on land), and much later, limbs to fins (wherein some mammals returned to the deep).

* [Spying on Whales](https://books.google.com/books/about/Spying_on_Whales.html?id=95yaDwAAQBAJ), by Nick Pyenson. The past, present, and future of whales, illuminated by modern DNA science.

* [Among Whales](https://books.google.com/books/about/Among_Whales.html?id=mUESAAAAYAAJ), by Roger Payne. Payne was part of the team that first discovered the structure of whalesong. This memoir recounts his life in science, and his immersion in the mystery and beauty of nature.

## External resources

* [The Human Impacts Database](https://anthroponumbers.org/). Useful quantities describing the interactions of humans with Earth's land, oceans, atmosphere, flora and fauna.

* [The Bionumbers Database](https://bionumbers.hms.harvard.edu/search.aspx). An incredibly handy collection of numbers from the molecular and cell biology literature.

* [Street-Fighting Mathematics: The Art of Educated Guessing and Opportunistic Problem Solving](https://sept.mit.edu/sites/default/files/Streetfighting%20Mathematics.pdf). This excellent free book by Sanjoy Mahajan (a Caltech alum!) teaches order-of-magnitude estimation in the same style that we will employ throughout the course. Essential reading for those curious to explore more advanced techniques than those we will cover.

* [Order-of-Magnitude Physics: A Textbook with Applications to the Retinal Rod and to the Density of Prime Numbers](https://thesis.library.caltech.edu/5338/1/Mahajan_s_1998.pdf). Mahajan's original Caltech PhD thesis, which later evolved into another excellent free textbook.

* [The Missing Semester of Your CS Education](https://missing.csail.mit.edu/), MIT

* [Be/Bi 103: Data Analysis in the Biological Sciences](http://www.bebi103.caltech.edu), Justin Bois/Caltech

* [Probability Distribution Explorer](https://distribution-explorer.github.io/index.html), Justin Bois

* [Statistics 110: Probability](https://projects.iq.harvard.edu/stat110/about), Joe Blitzstein/Harvard
