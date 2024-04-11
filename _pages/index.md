---
layout: page
title: Home
id: home
permalink: /
---
# Welcome!

I finally created this website (April 2024).  I'm still testing it though, so <span style="color:#f90185">it's going to be messy for at least a few days</span>. 

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  This website is where I process some inputs. Inputs are my experiences of things.
  <br>
  I do this in an Obsidian vault that I partially copy over here.
  <br>
  Here's an example [[imps|input]]. All inputs can be seen on a [[graph]].
  <br>
  <br>
  You can read more about me [[about|here]].
</p>

For information on the technical implementation of this website, see [[webtech|here]].

Now, the mess: I'm playing around with everything below the line!

---

<!-- TESTING -->

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
  {% assign all_notes_by_date = site.notes | sort: "datefirstcreated" | reverse %}
  {% for note in all_notes_by_date %}
    <li>
      {{ note.datefirstcreated }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a> 
    </li>
  {% endfor %}
</ul>

<strong>Alphabetical</strong>

<ul>
  {% assign alpha_notes = site.notes | sort: "title" %}
  {% for note in alpha_notes %}
    <li>
      <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a> 
    </li>
  {% endfor %}
</ul>

<strong>TEST FILTER for imps</strong>

<ul>
  {% assign test_notes2 = site.notes %}
  {% for note in test_notes2 %}
	  {% if note.title == "Imps" %}
	<li>
      {{ note.datefirstcreated }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a> 
    </li>
    {% endif %}
  {% endfor %}
</ul>

<strong>TEST ANOTHER FILTER for imps</strong>

<ul>
  {% assign test_notes5 = site.notes | where:"tags","test" %}
  {% for note in test_notes5 %}
	<li>
      {{ note.datefirstcreated }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a> 
    </li>
  {% endfor %}
</ul>


<strong>Notes by tag</strong>

<ul>
  {% assign all_notes_by_tag = site.notes | sort: "tags" %}
  {% for note in all_notes_by_tag %}
    <li>
      {{ note.datefirstcreated }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a> 
    </li>
  {% endfor %}
</ul>


