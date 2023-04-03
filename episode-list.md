---
layout: default
title: Episode List
permalink: /episode-list
date: 2023-04-02 14:15:00 -0000
categories: episodes introduction jolts
thumbnail: /_assets/title_card_300px_v01.png
---

<h1>Recent Episode</h1>

This is a list of the newest episodes: 

[Introduction]("/_podcasts/230314-112657-Ep00-00.mp3?raw=true")

<ul>
  ("/_assets/title_card_300px_v01.png")
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

This is a second line:
