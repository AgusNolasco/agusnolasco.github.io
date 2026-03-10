---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---

You can also find my articles on <a href="https://scholar.google.com/citations?user=sB0yPmMAAAAJ&hl=en">my Google Scholar profile</a>.

{% include base_path %}

{% for post in site.publications reversed %}

{% if post.paperurl %}
<h2><a href="{{ post.paperurl }}" target="_blank">{{ post.title }}</a></h2>
{% else %}
<h2>{{ post.title }}</h2>
{% endif %}

<p>
{{ post.authors }}<br>
<i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}
</p>

{{ post.content }}

<hr>

{% endfor %}
