---
layout: default
title: Lectures and labs

---

I would like to thank Prof. [Alexander Schwing](https://www.alexander-schwing.de/), Prof. [Aigou Han](https://beam.vt.edu/people/faculty/han.html), Prof. [Farzas Kamalabadi](https://ece.illinois.edu/about/directory/faculty/farzadk), and Prof. [Corey Synder](https://grainger.illinois.edu/about/directory/faculty/cesnyde2) for their support and lecture documents which I've based much of my own work on. 

Also, quick hint, icons are links to slides and video contents! 

{% comment %}
 <div class="card-columns">
    {% comment %}
    Sort the lectures by date, putting those without dates last
    {% endcomment %}
    {% assign lectures_by_date = site.lectures | sort: 'deliverydate', 'first' %}
    {% for l in lectures_by_date %}
        {% include lecture-card.html lecture=l %}
    {% endfor %}
</div>
{% endcomment %}

{% assign lectures_by_date = site.lectures | sort: 'deliverydate', 'first' %}
{% assign labs_by_date = site.labs | sort: 'deliverydate', 'first' %}


<section class="people row justify-content-between">
    <div class="col-md-7">
        <h3 class="pt-3"> Lectures </h3>
        {% for l in lectures_by_date %}
            {% include lecture-card.html lecture=l %}
        {% endfor %}
    </div>
    <div class="col-md-5">
        <h3 class="pt-3"> Labs </h3>
        {% for l in labs_by_date %}
            {% include lab-card.html lecture=l %}
        {% endfor %}
    </div>    
</section>