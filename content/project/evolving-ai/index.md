---
title: Evolving AI
summary: Model Learning with limited training data.
tags:
- Deep Learning
- Model Learning
- Knowledge Transfer
- Few Shot Learning
date: "2018-01-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: Link
  url: https://github.com/jabhinav/Model-Learning
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
In this project, we address the problem of re-training a deep neural network for a new class with limited training data (n to n+1 class learning) using a novel concept of Deep part embeddings (DPEs). DPEs are sub-networks of neuron activation extracted from a trained network identifying a visual and distinguishable element of a class. We identify visual elements that intuitively constitute a new class and extract the corresponding DPEs from the network pre-trained for the class sharing the identified visual element. 

Finally, we assemble them into a new network and re-train the model on limited samples of the new class and a subset of data from `n' classes to achieve high accuracy on the new class without significantly affecting the accuracy of n classes. We studied and generated results for DPE integration under two configurations- (i) sequential, when DPEs are sourced from different CNN architectures and (ii) shared; when DPEs are sourced from the same CNN architecture.
