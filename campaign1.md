---
layout: campaign
title: "Campaign 1"
permalink: /campaign1/
---

# Welcome to Campaign 1

This is the content of the Campaign 1 page. You can add text, images, links, and any other HTML or Markdown content here.

<ul class="post-list">
    {% for post in site.campaign1 %}
        <li>
            <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

            <h2>
                <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
            </h2>
        </li>
    {% endfor %}
</ul>
