---
layout: page
title: beranda
id: home
permalink: /
---

<div class="container">
<div class="left-column" markdown="1">
my first instinct when creating this repository was to call it an archive, but *archive* is such a loaded word — imbued with the sense of something unchanging, when this space will be (is?) anything *but*. (i want us to forever be mutable.)

this site is in every sense a [**digital garden**](https://maggieappleton.com/garden-history), but that specific metaphor-analogy just doesn't resonate with me as much — i don't have a green thumb. i don't care much to tend, or cultivate; all my life i've grown up in jakarta, anyway.

short-form platforms like twitter & bluesky are great for hashing out & expanding one's thoughts (communally, too!); but they're too ephemeral & temporal. at the same time, long-form platforms like substack & medium implicitly demand a polished form of writing when you hit publish, & don't tend to incentivize one going back & reflecting on their thoughts — relying more on newness & novelty, & doing so constantly.

_—but to write is to remember._

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
    max-width: 50em;
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
    font-size: 0.9em;
  }
  .right-column {
    flex: 30%;
    padding: 10px;
    box-sizing: border-box;
    font-size: 16px;
  }
</style>
