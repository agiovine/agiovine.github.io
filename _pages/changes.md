---
layout: page
title: "Changes from template"
permalink: /changes
---
I've made a few modifications from Maxime Vaillancourt's [Digital Garden Jekyll Template](https://github.com/maximevaillancourt/digital-garden-jekyll-template). These are listed here:

- Created separate page for graph and removed graph from individual notes pages (to avoid getting caught in graph zoom when scrolling on a notes page). This entailed:
	- creating \_layouts/graph.html
	- creating\_pages/graph.md
- Changed notes template to include YAML information about creation date (datefirstcreated); this entailed:
	- modifying \_layouts/note.html with page.datefirstcreated code