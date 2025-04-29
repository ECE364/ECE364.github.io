---
layout: default
title: Homeworks
---

Homework assignments can be found on the PrarieLearn site (link on main page). 

<table id="customers">
  <tr>
    <th> # </th>
    <th>Topic</th>
    <!-- <th>|Problems|</th> -->
    <th>Assigned</th>
    <th>Due</th>
    <!-- <th>Questions</th> -->
    <!-- <th>Solutions</th> -->
  </tr>
  {% for iteml in site.data.homework %}  
    {% assign item = iteml[1] %}
    <tr>
        <td>{{ item.num }}</td>
        <td> {{ item.topic }} </td>
        <!-- <td> {{ item.num-problems }} </td> -->
        <td> {{ item.assigned-date | date: "%b %d" }} </td>
        <td> {{ item.due-date | date: "%b %d" }} </td>
        <!-- <td> 
            {% if item.questions-link %}
            <a href="{{ site.base }}{{ item.questions-link }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Homework {{ item.num }} Questions"
                    title="Homework {{ item.num }} Questions"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
        </td> -->
        <!-- <td> 
            {% if item.solutions-link %}
            <a href="{{ site.base }}{{ item.solutions-link }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Homework {{ item.num }} Questions"
                    title="Homework {{ item.num }} Questions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}
        </td> -->
    </tr>        


  {% endfor %}

</table>

&nbsp;

Couple things to note about homeworks
- Homeworks are to be completed **individually** through PrairieLearn.
- Each homework is assigned when you have most (if not all) of the required knowledge to complete it.  **There is zero reason not to start the homework early.** Office hours are not provided on Mondays and HWs are due Monday night. Please plan ahead. 
- Most homeworks will consist of 3-4 novel problems. Each homework is weighted equally towards your final grade. 
- The homework average consists 25% of your final course grade. We will drop your lowest homework score. 
- It's a bad idea to skip homeworks. Homeworks and labs are where we get inspiration for exam problems. 

### Homework Logistics: How to submit

- All homeworks are administered and graded through PrairieLearn. Problems are mostly autograded, though there will be a few free-form responses that require manual grading.
- **Homeworks are due by 23.59.59 (11.59.59 PM)** of their due date (so midnight Monday night). In other classes, I used to make the deadline 6AM, but many students would stay up all night to do the homeworks and I want you guys to sleep. Again my intent is absolutely not to consume your weekend. You have 11 days to complete the homework and the knowledge necessary to complete the problems at the time of assignment. Start the assignment early, go to OHs if you get stuck, and you'll have no problem finishing the homework quickly. 
- You **should not** use Canvas to keep track of homeworks or any other course policies and logistics. **Canvas is a gradebook, that's all.**  
- You will be registered with PrairieLearn using your university email address. If you can't access PrairieLearn let the course staff know. 
- Late homeworks are penalized at a rate of 1 point/hour that they are late. We will not discuss late homeworks in OHs. We have a small staff and we need to prioritize current homeworks in OH. 

### Homework Grading Policies: 

- **Homeworks** are graded by the entire course staff, both manually and with auto-grader software. 
- Under normal circumstances, all homework should be graded within two weeks of submission (this pertains more to manually graded portions of homeworks). However, the course staff members also have significant responsibilities and may take longer to grade the homeworks. This is all to say one thing: **homeworks should not be used to check your mastery of the material.** Most (if not all) problems will have some autograded portions, so you should have early indications of if you understand a particular concept. If you get stuck, use OHs! 
- Homework grades are **not** a proof of correctness and cannot be used to argue for correctness on an exam. 
- Partial credit is given depending on the question. Most auto-graded assignments will not have partial credit but manually graded assignments might. PrairieLearn should indicate when partial credit is given for an auto-graded assignment.

### Allowable resources

- Textbooks and online documentation are allowed to be used with the homeworks.  
- You are not allowed to use generative AIs for the homeworks. I totally get that lots of people find generative AI to be a useful [rubber duck](https://en.wikipedia.org/wiki/Rubber_duck) when coding, but I do not believe that is the way most people are using it. I totally understand the philosophical argument, but I've been doing this a while now, and I firmly believe eliminating all struggle from learning harms students from becoming more intelligent the same way eliminating struggle from exercise eliminates any strength gains. And there's more research coming out that supports [this point of view](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4895486). 
