---
layout: page
title: Home
id: home
permalink: /
---

# Bem-vindo!✨

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
Comece por <span style="font-weight: bold">[[Outra vez, olá]]</span>
</p>

Esse site foi criado para você.

Caso não retorne contato dentro de duas semanas, ficará indisponível.
Se for o caso, agradeço por ter feito parte da minha vida.
Desejo o melhor para você.

Após a leitura da publicação "[[Outra vez, olá]]", comece em [[Estrelas]]

<strong>Últimas notas publicadas</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
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
