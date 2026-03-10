---
layout: single
title: "Students"
permalink: /students/
author_profile: true
---

{% include base_path %}

{% for post in site.students reversed %}
  <h2>{{ post.title }}</h2>

  <p>
    {{ post.type }}<br>
    <i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}
  </p>

  {{ post.content }}

  <hr>
{% endfor %}
