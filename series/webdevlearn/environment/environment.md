---
layout: page
title: Environment
permalink: /webdevlearn/env
nav_order: 1
has_toc: false
parent: WebDev
has_children: true
topic: Env
category: webdevlearn
---

Here are some handy tools:
{{ page.topic }}

1. stuff
2. more stuff

<ul>
  {% for post in site.posts %}
    {% if post.topic contains  page.topic%}
      <li>
        <span>{{ post.topic }} - </span><a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
