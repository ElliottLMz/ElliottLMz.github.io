---
title: "My Blog"
layout: page
permalink: /blog
---

# Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <p>
        <a href="{{ post.url }}">{{ post.title }}</a>&nbsp;&nbsp;
          <span>{{ post.date | date_to_string }}</span>
      </p>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>