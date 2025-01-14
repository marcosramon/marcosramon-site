---
layout: page
title: Home
id: home
permalink: /
---

# Olá! 👋🏼

![](/assets/images/gephi2.png)

Meu nome é Marcos Ramon. Sou professor de Filosofia no IFB, pesquisando estética e cibercultura.

- 😊 [Sobre o autor](https://marcosramon.net/sobre){: .internal-link}
- 📂 [Arquivo](https://marcosramon.net/arquivo){: .internal-link}
- 📘 [Livros publicados](https://marcosramon.net/livros){: .internal-link}
- 🎙️ [Podcast](https://open.spotify.com/show/1smphr2Sl3kHncMYB984rc?si=Ds7GV4oNQnGxsm-bxYvasA&nd=1){: .internal-link}
- 📺 [YouTube](https://www.youtube.com/conexaofilosofica){: .internal-link}
- 😍 [Apoie](https://marcosramon.net/apoie){: .internal-link}

Inscreva-se na [newsletter](https://marcosramon.substack.com/){: .internal-link} para receber atualizações por email. 😉

<strong>Mais recentes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "date" | reverse %}
  {% for note in recent_notes limit: 12 %}
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
