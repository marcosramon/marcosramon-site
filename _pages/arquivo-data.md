---
layout: page
title: Arquivo com todos os posts
permalink: /arquivo-data
---

## Arquivo com todos os posts
Aqui você encontra todos os posts publicados no site:

<ul>
    {% assign all_notes = site.notes | sort: "date" | reverse %}
    {% for note in all_notes %}
      <li>
        {{ note.date | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
      </li>
    {% endfor %}
</ul>

