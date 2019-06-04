---
date: 2019-06-02
title: Fitzpatrick 2016
categories:
  - Environmental metagenomics
description: BLASTing AMR genes against a local db of metagenomic reads
type: Document
related_post:
comments: true
doi: 10.1093/femsec/fiv168
---

## Summary

|||
|----|----|
|category|read-based|
|platform|not stated|
|open source|true|
|reproducible|false|
|documented|true|


## Database

This protocol uses the Antibiotic Resistance Database ([ARDB](https://ardb.cbcb.umd.edu/)). An exact version number was not given but total number of genes was listed as 23,137, encoding resistance to 249 antibiotics. These genes were then subsampled so that each AMR gene type had a single representative, resulting in 381 genes. These 381 reference AMR genes that are used in this protocol are available in FASTA format in the supplemental dataset 2 of the [paper](https://academic.oup.com/femsec/article/92/2/fiv168/2484737#82440962).


## Protocol

* Step 1

A local file of AMR genes was created by downloading all sequence data from the ARDB

* Step 2

A single representative AMR gene was selected for each AMR gene type, in addition the blaNDM gene sequence was included as this was absent from the ARDB

* Step 3

All 381 AMR genes were treated as query sequences and compared to a local metagenomic database built from the metagenomic reads. Comparisons were performed using BLASTp with a cutoff expectation (E) value of <10<sup>−10</sup>

* Step 4

A read was annotated as a potential AMR gene if its top high-scoring segment pair (HSP) had a percent identity >90% and the HSP length was greater than 60% of the query AR gene.

* Step 5

The total number of reads that pass these criteria for each AMR gene was recorded and labeled as AMR reads. The relative abundance for each AR gene in the metagenome was calculated by dividing the specific number of AMR reads by the total number of reads in that metagenome.


## Citation

The paper(s) documenting this protocol:

* D. Fitzpatrick and F. Walsh. [Antibiotic resistance genes across a wide variety of metagenomes. FEMS MICROBIOLOGY ECOLOGY. 2016](https://academic.oup.com/femsec/article/92/2/fiv168/2484737)
