---
layout: page
title: Home
id: home
permalink: /
description: ciao
---
Ciao! I am Alberto an hardware designer & music producer based in stockholm, sweden.

<img src="{{ site.baseurl }}/assets/img/me_el_chalten.jpeg" /><br>

I am currently Senior Electronics Engineer at [teenage engineering](https://teenage.engineering/).

Checkout my [[projects]]


<strong>Recently updated notes</strong>

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
