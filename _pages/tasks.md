---
layout: default
title: Задачи по программированию
permalink: /tasks/
---

<section class="recent-posts">

    <div class="section-title">

        <h2>
            <span>
                Задачи по программированию
            </span>
        </h2>

    </div>

    <div class="row listrecent">

        {% for post in site.posts %}

        {% if post.type == 'task' %}

        {% include postbox.html %}

        {% endif %}

        {% endfor %}

    </div>

</section>

