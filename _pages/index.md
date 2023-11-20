---
layout: page
title: 
id: home
permalink: /
description: ciao
---
ciao! 
I am alberto,  hardware designer & music producer based in stockholm, sweden.  
Currently, I am a senior electronics engineer at [teenage engineering](https://teenage.engineering/).

from here you can:  

- explore the [[projects]] I worked on
- listen to my unreleased [[music]]
- [[inspiration| get inspired]]
- learn more [[about| about me]].  


<strong>Recently updated notes</strong>
<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 3 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>


