---
layout: default
title: Writeups
permalink: /writeups/
---
<section class="card">
  <h1>Writeups</h1>
  <p>Reverse engineering notes, malware analysis walkthroughs, and challenge solutions.</p>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a><br>
        <span class="post-meta">{{ post.date | date: "%B %d, %Y" }}</span><br>
        <span>{{ post.excerpt | strip_html | truncate: 200 }}</span>
      </li>
    {% endfor %}
  </ul>
</section>

