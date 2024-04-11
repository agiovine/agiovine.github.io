---
layout: page
title: "Website technical details"
permalink: /webtech
---
# Website technical details

This website was generated from the [Digital Garden Jekyll Template](https://github.com/maximevaillancourt/digital-garden-jekyll-template) by [Maxime Vaillancourt](https://github.com/maximevaillancourt), with much appreciation!

I've made a few modifications:

- Changed where the graph appears on the website:
	- I created a separate page for the graph (new files: <span style="color:#f90185">_layouts/graph.html</span> and <span style="color:#f90185">_pages/graph.md</span>).
	- I modified <span style="color:#f90185">_layouts/note.html</span> to remove the graph from the bottom of individual notes pages.  Notes pages now instead include a link to the graph page (previous bullet) in the side section (under "Notes mentioning this note").  I did this because the graph can be annoying when you are scrolling on a mobile device (you get caught in the zoom).
- Changed notes template to include YAML information about creation date; this entailed modifying <span style="color:#f90185">_layouts/note.html</span> with page.datefirstcreated code.
- Smaller aesthetic chnages:
	- Unmentioned notes (notes with no backlinks): the side section text (under "Notes mentioning this note") is also contained in a gray box (like mentioned notes).  This helps visual separation of the side section from the main content.