---
layout: post
title: "Libraries to visualize taxonomic trees"
description: ""
category: visualization
tags: [python,visualization,taxonomy,trees]
---
{% include JB/setup %}

Miniproject to be done: a script to show a _biodiversity_ of metagenomic sample on a taxonomic tree. 


There are quite a few options to visualize phylogenetic trees in a programmatic way. See [summary by Kat Holt](http://bacpathgenomics.wordpress.com/2012/05/25/displaying-data-associated-with-phylogenetic-trees/). Out of three (four) ways mentioned [E.T.E Python library](http://ete.cgenomics.org/) looks as a best starting point. [E.T.E original paper](http://www.biomedcentral.com/1471-2105/11/24) has been [cited 31 times](http://scholar.google.pl/scholar?hl=pl&lr=&cites=8265169148820148043&um=1&ie=UTF-8&sa=X&ei=dHWZUL2VFYPdtAbQoYDwAQ&ved=0CDgQzgIwAQ), many times by other software packages. 

Webpage seems to be abandoned, but Google Group is active and it seems the package in under continous development (see [this thread, as a example](https://groups.google.com/forum/?fromgroups=#!topic/etetoolkit/9vKY_GgIzkA) ). 

While classic biodiversity analysis in metagenomic studies doesn't involve making real phylogenetic trees (well, it often does, but given small length of sequences in the alignment, resulting tree is not that accurate in more general terms), I have some ongoing projects which would require large scale visualization and analysis of trees. Coupling E.T.E-based script with [Bio.Phylo](http://www.biomedcentral.com/content/pdf/1471-2105-13-209.pdf) might be interesting path to explore. 

Other things found in this area is [ScripTree](http://lamarck.lirmm.fr/scriptree/) and [DendroPy](http://bioinformatics.oxfordjournals.org/content/26/12/1569.full). The former is Tk, the latter again Python.

BTW, to parse results from _mothur_ I would need to rewrite [Pierre's script](http://www.biostars.org/p/52895/) to Python.