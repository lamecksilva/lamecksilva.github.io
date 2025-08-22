---
layout: default
title: "CS App"
---

### Computer Systems: A Programmer's Perspective

Minhas anotações e resumos da leitura e estudos desse livro.

<h1>{{ page.title }}</h1>

{% assign siblings = site.pages | where: "dir", page.dir %}

<ul>
  {% for p in siblings %}
    {% unless p.url == page.url or p.name == 'index.md' %}
      <li>
        <a href="{{ p.url | relative_url }}">
          {{ p.title | default: p.name | replace:'.md','' | replace:'.html','' }}
        </a>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
