---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! Thank you for coming here. 🌱

This is a tiny place for my [[1,1 definition of evergreen notes|Evergreen notes]]

Most of the input that I consume goes through Obsidian or my Analog Zettelkasten, and then, appears here.

[[Evergreen notes moc|Start here]]

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 30 %}
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
