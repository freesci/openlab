---
layout: post
title: "Visual summaries of proteins"
description: ""
category: project
tags: [alignment,visualization,proteins]
---
{% include JB/setup %}


This page is devoted to various ways of visually summarizing multiple sequence alignments (mainly protein ones). 

### MSA-VIS - Django based server for visualization of protein MSAs

The purpose of this project was to build a complete tool that overlays conservation data with chemical properties of aminoaci
d residues. The proof of concept has been developed before and released as Aln2Plot tool (http://toolkit.tuebingen.mpg.de/aln
2plot). In this version the visual side has been substantially improved and additionally, prediction of secondary structures 
has been added as an option. 

Fragment of the output: 



_Authors:  Małgorzata Habich, Monika Maksymiuk, Marta Styczyńska, Katarzyna Wręczycka (all four did the coding, in alphabetical order) and PS (idea, design, supervision)_


### Visualization of internal repeats in sequences

There're many protein families that have internal repeats (like TPR, Armadillo, ankyrin etc.). In some proteins, the repeats 
are separated by other segments, resulting in mosaic-like structure. In an attempt of making sense of such mosaics, I've buil
t a tool with Processing that implemented the idea behind [The Shape of Song](http://www.turbulence.org/Works/song/method/method.html) – visualization method developed by Martin Wattenberg, researcher at IBM. Resulting visualization is shown below. 


Repeats are colored according to repeat type and are connected according to repeat family. If you think about it in terms of 
SCOP (Structural Classification of Proteins) hierarchy, colors represent class, while arcs connect superfamilies. The longer 
and more complicated analysed sequence is, the more useful this approach seems to be, so for short proteins typical domain bu
bbles would work better.

The source code is [available at GitHub](https://github.com/freesci/java-protein-domain-visualization) (hasn't been updated in a while). The tool has been incorporated into server Domain Annotation of Trimeric Autotransporter Adhesins [DATAA](http://toolkit.tuebingen.mpg.de/dataa) and subsequently published: 



_Authors: AL (inspiration,design optimization), PS (coding, design)_

### Time-lapse analysis of alignments

In attempt of understanding how certain positions of large protein MSA behave in respect to the known structure I did a time-
lapse analysis of its fragments. In essence, I took the alignment, chose a master sequence that correspond to a known structu
re, removed all columns with gaps in the master sequence, and visualized fragments of the alignment (sliding window with 15 s
equences) with [Weblogo](http://weblogo.berkeley.edu/) – software for preparing sequence logos from alignments. On the video
 below you can see:

* two boxes showing the same template structure (second is just rotated); size of C-alpha atoms correspond to overall conse
rvation at that position; first few residues do not have corresponding positions in the alignment
* sequence logo of actual alignment window
* sequence logo of the whole alignment – as a reference

Source code will be uploaded to GitHub soon.


_Authors: PS (all stuff)_


