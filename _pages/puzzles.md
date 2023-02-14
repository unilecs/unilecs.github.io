---
layout: default
title: Головоломки
permalink: /puzzles/
---

<section class="recent-posts">

    <div class="section-title">

        <h2>
            <span>
                Головоломки
            </span>
        </h2>

    </div>

    <div class="row listrecent">

        {% for post in site.posts %}

        {% if post.type == 'puzzle' %}

        {% include postbox.html %}

        {% endif %}

        {% endfor %}

    </div>

</section>

