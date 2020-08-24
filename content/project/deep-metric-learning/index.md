---
title: Deep Metric Learning
summary: Video Representation Learning for Fine-Grained Scene Recognition and Retrieval.
tags:
- Deep Learning
- Event Recognition
- Loss Formulation
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
  url: https://github.com/jabhinav/Deep-Video-Understanding
url_code: ""
url_pdf: "https://github.com/jabhinav/Deep-Metric-Learning-for-Video-Understanding/blob/master/Radial_Loss_Preprint.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
We proposed Pentuple Loss and an improved Radial Loss in the domain of deep metric learning to learn an order-preserving fine-grained similarity metric. The loss exploits the concept of 'Quadlet Sampling' to mine data where each training sample is a tuple of query f(q), positive f(p), intermediate f(i) and negative samples f(n). The loss maintains relative distance between samples of the quadlet in the embedding space such that for a given query sample (say of sub-class ‘S1’ in class ‘C1’), gradients of the loss move the negative samples (say, of class ‘C2’) away from class ‘C1’ containing other positive samples (sub-class ‘S1’ in class ‘C1’) and intermediate samples (sub-class ‘S2’ in class ‘C1’). The loss takes a step further and also achieves finer separation between samples of different sub-classes within a class. We demonstrated the performance of our loss in the tasks of query-based image retrieval and in the two novel tasks of ***video critical scene recognition*** and ***fine-grained video retrieval***. 

The research is motivated by the requirement in digital media where recognition of critical scenes in videos are required for smart placement of brand advertisements. Such critical scenes raise viewer anxiety and are a part of some parent activity. We distinguish them from the rest of the temporally overlapping video event using the similarity metric that learns the required representation of critical and non-critical scenes of a video clip.
