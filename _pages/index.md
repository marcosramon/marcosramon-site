---
layout: page
title: Home
id: home
permalink: /
---

# Olá! 🌱

![](/assets/images/gephi2.png)

Meu nome é Marcos Ramon. Sou professor de Filosofia no IFB, pesquisando estética e cibercultura.

- 😷 [Sobre o autor](https://marcosramon.net/sobre)
- 📂 [Arquivo](https://marcosramon.net/arquivo)
- 📘 [Livros publicados](https://marcosramon.net/livros) 
- 🎙️ [Podcast](https://open.spotify.com/show/1smphr2Sl3kHncMYB984rc?si=Ds7GV4oNQnGxsm-bxYvasA&nd=1)
- 😍 [Apoie](https://marcosramon.net/apoie)

Inscreva-se na [newsletter](https://marcosramon.substack.com/) para receber atualizações por email. 😉

<strong>Mais recentes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "date" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.date | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
