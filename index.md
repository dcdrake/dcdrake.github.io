---
layout: default
---
<p class="intro">
  Observations on software and the people who build it—how teams think, why tools get adopted, and what organizations reveal about themselves through code.
</p>

<ul class="post-list">
  {% for post in site.posts %}
  <li class="post-item">
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    <h2 class="post-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    {% if post.excerpt %}
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    {% endif %}
  </li>
  {% endfor %}
</ul>
