---
layout: default
title: Home
---
<section class="hero card">
  <p class="eyebrow">Reverse Engineering / Malware Analysis / Defensive Tradecraft</p>
  <h1>Writeups and notes from the lab.</h1>
  <p class="lede">
    A home for reverse engineering writeups, malware analysis notes, small security projects,
    and practical lessons worth keeping.
  </p>
  <a class="button" href="{{ '/writeups/' | relative_url }}">Read the writeups</a>
</section>

<section class="grid">
  <article class="card">
    <h2>Writeups</h2>
    <p>Structured analysis notes, challenge writeups, and sample deep-dives with screenshots and defender takeaways.</p>
    <a href="{{ '/writeups/' | relative_url }}">Browse posts</a>
  </article>
  <article class="card">
    <h2>Projects</h2>
    <p>Tools, scripts, workflows, and lab experiments that support malware analysis and detection engineering.</p>
    <a href="{{ '/projects/' | relative_url }}">See projects</a>
  </article>
  <article class="card">
    <h2>Tips</h2>
    <p>Short practical notes for analysts, defenders, and curious builders who want usable cybersecurity advice.</p>
    <a href="{{ '/tips/' | relative_url }}">Read notes</a>
  </article>
</section>

<section class="card">
  <h2>Latest writeups</h2>
  <ul class="post-list">
    {% for post in site.posts limit:3 %}
      <li>
        <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a><br>
        <span class="post-meta">{{ post.date | date: "%B %d, %Y" }}</span><br>
        <span>{{ post.excerpt | strip_html | truncate: 180 }}</span>
      </li>
    {% endfor %}
  </ul>
</section>

