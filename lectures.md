---
layout: default
title: Lectures

---

I would like to thank Prof. [Alexander Schwing](https://www.alexander-schwing.de/), Prof. [Aigou Han](https://beam.vt.edu/people/faculty/han.html), Prof. [Farzas Kamalabadi](https://ece.illinois.edu/about/directory/faculty/farzadk), and Prof. [Corey Synder](https://grainger.illinois.edu/about/directory/faculty/cesnyde2) for their support and lecture documents which I've based much of my own work on. 

Also, quick hint, icons are links to slides and video contents! 

<table id="customers">
  <tr>
    <th> # </th>
    <th>Title</th>
    <th>Date</th>
    <th>Slides</th>
    <th>Recording</th>
    <!-- <th>Solutions</th> -->
  </tr>
  {% for iteml in site.data.lecture %}  
    {% assign item = iteml[1] %}
    <tr>
        <td>{{ item.num }}</td>
        <td> {{ item.title }} </td>
        <td> {{ item.deliverydate | date: "%b %d" }} </td>
        <td> 
            {% if item.link-slides %}
            <a href="{{ site.base }}{{ item.link-slides }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Lecture {{ item.num }} slides"
                    title="Lecture {{ item.num }} slides"
                    src="{{ site.base }}/img/icons/slide_clean_3.png" />
            </a>
            {% endif %}
        </td>
        <td> 
            {% if item.link-recording %}
            <a href="{{ site.base }}{{ item.link-recording }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Lecture {{ item.num }} recording"
                    title="Lecture {{ item.num }} recording"
                    src="{{ site.base }}/img/icons/lecture_recording_3.png" />
            </a>
            {% endif %}
        </td>
    </tr>        


  {% endfor %}

</table>