---
title: Data Transformation
summary: 
tags:
- Symbolic/Statistical Program Synthesis
- Deep Learning
- Reinforcement Learning
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
  url: https://github.com/jabhinav/Reinforcement-Learning-for-Program-Synthesis
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

***Problem Statement***: Given a small subset of input samples, collect corresponding output samples from the user and learn a transformation routine that converts provided data into user-intended format.

***Motivation***: The idea is to facilitate end users, mostly non-experts, with a Programming-by-example, PbE system that captures the user intention and applies to all the provided samples with minimum intervention.

***What exists in the prior-art?*** Most papers in literature tackle the problem using a symbolic program synthesis approach, where the underlying model, with the help of a pre-defined set of atomic functions from an underlying Domain Specific Language, synthesizes the required transformation program (seq of functions). Symbolic models follow a divide-and-conquer strategy to break the problem of output generation from input into further sub-problems, each sub-problem focusing on using an atomic function to generate a specific portion of output from input.

***Key aspects for rule-based (symbolic) systems***:
- Independence of problems: We decouple the problem of generating the output string into independent sub-problems of generating different parts of the output from input. Logic for generating one part of the output string is completely independent of generating another disjoint substring of the output string.
- Number of possible sub-problems is quadratic: We enumerate all possible decompositions of the output string using Directed Acyclic Graph, DAG representation. It allows us to decompose the problem of generating the output string into a quadratic number of independent sub-problems of generating different substrings of the output string.
- DAG: Comprises of 'nodes' corresponding to every position within the output string and an 'edge' correspond to sub-string of the output contained within the positions marked by its node pairs. We further annotate each edge with all sets of atomic operations that can generate the corresponding substring from the input.
- Enumerates all simple paths from source node to target node, refering to the transformation programs comprised of sequences of atomic operations. 
- Ranks them using heuristics or Machine Learning models to provide top-k programs to the user.

***Drawbacks***:  For complex transformations, DAG becomes untraceable as the number of sub-problems increases dramatically and enumerative strategy of symbolic systems becomes computationally expensive. Additionally, with noise present in the data, symbolic systems fail terribly.

***Why Stastical Systems?*** Thus, a deep learning based solution robust to noise and able to work with complex transformations using a more expressive DSL in real-time is proposed.
