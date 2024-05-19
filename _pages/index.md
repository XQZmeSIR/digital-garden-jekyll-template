---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! Thank you for coming here. 🌱

This is a tiny place for my [[1,1 definition of evergreen notes|Evergreen notes]]

Most of the input that I consume goes through Obsidian or my Analog Zettelkasten, and then, appears here.

[[Evergreen notes moc|Start here]] to find out more about Evergreen notes.

Also check out my guide: [[Как настроить Zotero Integration plugin в Obsidian раз и навсегда]]

Maps of Content 🗺️: <br>
- [[Mini-Essays MOC]]
- [[Memory MOC]]
- [[Learning MOC]]
- [[Thinking MOC]]
- [[Cognitive biases MOC]]
- [[Concepts MOC]]
- [[PKM MOC]]
- [[Time-management MOC]]
- [[Languages MOC]]
- [[Quotes MOC]]


<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 10 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
