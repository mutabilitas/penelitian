---
layout: default
title: Home
id: home
permalink: /
---

<div class="container">
<div class="left-column" markdown="1">
## Welcome! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>

This digital garden template is free, open-source, and [available on GitHub here OMGGGG?????](https://github.com/maximevaillancourt/digital-garden-jekyll-template).

The easiest way to get started is to read this [step-by-step guide explaining how to set this up from scratch](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll).

</div>

<div class="right-column">
<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>
</div>
</div>

<style>
  .wrapper {
    max-width: 46em;
  }
.container {
    display: flex;
    flex-direction: row;
    max-width: 100%;
    margin: 0 auto;
  }
  .left-column {
    flex: 70%;
    padding: 10px;
    box-sizing: border-box;
  }
  .right-column {
    flex: 30%;
    padding: 10px;
    box-sizing: border-box;
    font-size: 16px;
  }
</style>
