---
layout: page
title: "Changes from template"
permalink: /changes
---
I've made a few modifications from Maxime Vaillancourt's [Digital Garden Jekyll Template](https://github.com/maximevaillancourt/digital-garden-jekyll-template). These are listed here:

- Changed where the graph appears on the website:
	- I created a separate page for the graph (new files: <span style="color:#f90185">_layouts/graph.html</span> and <span style="color:#f90185">_pages/graph.md</span>).
	- I modified <span style="color:#f90185">_layouts/note.html</span> to remove the graph from the bottom of individual notes pages and instead include a link to the graph on the side (under "Notes mentioning this note").
- Changed notes template to include YAML information about creation date; this entailed modifying <span style="color:#f90185">_layouts/note.html</span> with page.datefirstcreated code.