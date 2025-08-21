---
layout: default
title: "CS App"
---

### Computer Systems: A Programmer's Perspective

Minhas anotações e resumos da leitura e estudos desse livro.

<h1>{{ page.title }}</h1>

<ul>
  {% assign current_dir = page.url | replace: 'index.html','' %}
  {% for p in site.pages %}
    {% if p.url contains current_dir and p.url != page.url %}
      <li>
        <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
