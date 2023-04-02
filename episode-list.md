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

![Introduction]("/_podcasts/230314-112657 - Ep 00-00.mp3")

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

This is a second line:

<div class="includes-grid">
  {% for episode in site.data.podcast-list %}
	<li>
	{{ post.excerpt }}
	</li>
 {% include podcast.html podcast_id="123456789" %>
 {% include youtube.html youtube_id="987654321" %}
</div>