---
title: Coherent Visual Description of Textual Instructions
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
  url: https://github.com/jabhinav/IBM-project
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
In this project, following multi-stage framework was developed to provide visual aid for a sequence of text based instructions in the form of coherent images associated with each of them - (a) For each instruction, visualisable phrases consisting of head action verbs and noun phrases are mined using standard practices like POS tagging, Dependency parsing and Co-reference resolution. (b) For each visualisable phrase, an API query is made to retrieve a set of images from a dataset crawled from sources such as WikiHow, Flickr, Google etc. Phrases and images together dictate the action being conducted in the instruction. (c) Across instructions sharing common information in the form of latent/non-latent entities, coherency is maintained using a graph based matching method utilising Dijkstra's algorithm. A user study was conducted to validate improvement in understanding of text instructions and resemblance to actual ground truth.
