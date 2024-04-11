---
layout: page
title: Home
id: home
permalink: /
---
# Welcome!

I finally created this website (April 2024).  I'm still testing it though, so it's going to be messy for at least a few days. 

<!-- Testing comment here -->

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  This website is where I process some inputs. Inputs are my experiences of things.
  <br>
  I do this in an Obsidian vault that I partially copy over here.
  <br>
  Here's an example [[imps|input]].
  <br>
  <br>
  You can read more about me [[about|here]].
</p>

This website was generated from the [Digital Garden Jekyll Template](https://github.com/maximevaillancourt/digital-garden-jekyll-template) by [Maxime Vaillancourt](https://github.com/maximevaillancourt), with much appreciation! I've made a few changes ([[changes|tracked here]]).

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<strong>Notes by date created</strong>

<ul>
  {% assign recent_notes2 = site.notes | sort: "datefirstcreated" | reverse %}
  {% for note in recent_notes2 %}
    <li>
      {{ note.datefirstcreated }}: <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a> 
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
