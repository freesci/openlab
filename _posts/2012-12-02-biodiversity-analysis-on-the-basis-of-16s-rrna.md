---
layout: post
title: "Biodiversity analysis on the basis of 16S rRNA"
description: ""
category: bioinformatics
tags: [biodiversity,metagenomics,16S]
---
{% include JB/setup %}

There are many papers describing bias of amplification of 16S gene and resulting bias in assessment of biodiversity. However some interesting recent publications expand the story.

There's a nice research on [including number of 16S gene copies per genome into assessment of biodiversity](http://www.ploscompbiol.org/article/info%3Adoi%2F10.1371%2Fjournal.pcbi.1002743) Proportions of different genera is changed after including such information into analysis (see also the [key figure](http://www.ploscompbiol.org/article/info:doi/10.1371/journal.pcbi.1002743?imageURI=info:doi/10.1371/journal.pcbi.1002743.g005) from that paper). 

Quite new idea about using marker gene for biodiversity assessment came with [EMIRGE software](http://www.biomedcentral.com/content/pdf/gb-2011-12-5-r44.pdf) which reconstructs full 16S gene from shotgun sequencing (result is perfectly suitable biodiversity analysis). Reconstruction (as opposed to de novo assembly) captures many more copies of 16S gene, therefore it should be a better than similarity based methods. Early tests show reconstruction is better than amplification, altough my impression is that it wasn't that thouroughly tested as I would like. There are two other approaches to gene reconstruction from shotgun data ([this](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0039948) and [this](http://www.sciencedirect.com/science/article/pii/S0923250812000964)) but without working piece of code available I cannot say anything about validity of their approach.

In addition to 16S rRNA gene, other markers are considered for biodiversity analysis, most interesting being protein-conding genes (like [recA or rpoB](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0018011)). [Comparison of rpoB with 16S](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0030600) results in better recall using protein-coding gene than ribosomal gene, however more testing is needed, especially to include less prominent candidates. Introductory work has been published recently - authors use ORFs encoding known proteins and roughly 1000 of their homologs in known bacteria genomes to construct [a large phylogenetic tree from multi-protein alignment](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0023214). That is quite a neat idea, although the recurring question is about HGT. 

##References:
* Kembel SW, Wu M, Eisen JA, Green JL (2012) Incorporating 16S Gene Copy Number Information Improves Estimates of Microbial Diversity and Abundance. PLoS Comput Biol 8(10): e1002743. doi:10.1371/journal.pcbi.1002743
* Miller CS, Baker BJ, Thomas BC, Singer SW, Banfield JF. EMIRGE: reconstruction of full-length ribosomal genes from microbial community short read sequencing data. Genome Biol. 2011;12(5):R44.
* Fan L, McElroy K, Thomas T (2012) Reconstruction of Ribosomal RNA Genes from Metagenomic Data. PLoS ONE 7(6): e39948. doi:10.1371/journal.pone.0039948
* Johan Bengtsson, Martin Hartmann, Martin Unterseher, Parag Vaishampayan, Kessy Abarenkov, Lisa Durso, Elisabeth M. Bik, James R. Garey, K. Martin Eriksson, R. Henrik Nilsson, Megraft: a software package to graft ribosomal small subunit (16S/18S) fragments onto full-length sequences for accurate species richness and sequencing depth analysis in pyrosequencing-length metagenomes and similar environmental datasets, Research in Microbiology, Volume 163, Issues 6–7, July–August 2012, Pages 407-412, ISSN 0923-2508, 10.1016/j.resmic.2012.07.001.
* Wu D, Wu M, Halpern A, Rusch DB, Yooseph S, et al. (2011) Stalking the Fourth Domain in Metagenomic Data: Searching for, Discovering, and Interpreting Novel, Deep Branches in Marker Gene Phylogenetic Trees. PLoS ONE 6(3): e18011. doi:10.1371/journal.pone.0018011
* Vos M, Quince C, Pijl AS, de Hollander M, Kowalchuk GA (2012) A Comparison of rpoB and 16S rRNA as Markers in Pyrosequencing Studies of Bacterial Diversity. PLoS ONE 7(2): e30600. doi:10.1371/journal.pone.0030600
* Kembel SW, Eisen JA, Pollard KS, Green JL (2011) The Phylogenetic Diversity of Metagenomes. PLoS ONE 6(8): e23214. doi:10.1371/journal.pone.0023214