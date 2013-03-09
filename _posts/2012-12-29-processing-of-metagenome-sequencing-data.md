---
layout: post
title: "Processing of metagenome sequencing data"
description: "workflow notes"
category: bioinformatics
tags: [metagenomics,R,ngs]
---
{% include JB/setup %}

Ongoing notes on the processing of shotgun metagenome sequencing data.

1. Quality assessment


2. Assessment 


samtools view -bS aqq.sam >aqq.bam
samtools sort aqq.bam aqq.sorted
samtools index aqq.sorted.bam
samtools idxstats aqq.sorted.bam >aqq.idxstats
perl -e 'while(<>){chomp;@a=split "\t", $_; $b+=$a[2]; $c+=$a[3];}
print "$b - $c\n";' aqq.idxstats
