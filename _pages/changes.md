---
layout: page
title: "Changes from template"
permalink: /changes
---
I've made a few modifications from Maxime Vaillancourt's [Digital Garden Jekyll Template](https://github.com/maximevaillancourt/digital-garden-jekyll-template). These are listed here:

- Created separate page for graph and removed graph from individual notes pages (to avoid getting caught in graph zoom when scrolling on a notes page); this entailed:
	- creating <span style="color:#f90185">_layouts/graph.html</span>
	- creating <span style="color:#f90185">_pages/graph.md</span>
- Changed notes template to include YAML information about creation date (datefirstcreated); this entailed:
	- modifying <span style="color:#f90185">_layouts/note.html</span> with page.datefirstcreated code