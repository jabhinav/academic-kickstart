---
title: Visual Cues for Text
summary: Provide visual aid for a sequence of text based instructions.
tags:
- Deep Learning
- Text-to-Image
- Graph Matching
date: "2016-05-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: Link
  url: https://github.com/jabhinav/Coherent-Visual-Description-of-Textual-Instructions
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Text is the easiest means to record information and can communicate a fact, argument or logical sequence. But it need not always be the best means for understanding a concept. Images are more evocative than text and invoke lateral thinking, objectivity and global context. By establishing a better balance between the two, comprehension of the textual instructions becomes easier. 

We developed a multi-stage framework to provide visual aid for a sequence of text-based instructions in the form of coherent images. For each instruction, the framework mines visualisable phrases consisting of head action verbs and noun phrases (denoting actions, objects and subjects) using standard practices like POS tagging, Dependency parsing and Co-reference Resolution. For each visualisable phrase, an API query is then made to retrieve a set of images from a dataset crawled from sources such as WikiHow, Flickr, Google etc. Across instructions sharing common information in the form of latent/non-latent entities, we maintain coherency using a graph-based matching method that utilises Dijkstra's algorithm. Phrases and images then together dictate the action being conducted in the instruction.
