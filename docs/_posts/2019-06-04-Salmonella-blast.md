---
date: 2019-06-03
title: Carroll 2017
categories:
  - Isolate data, Salmonella
description: Salmonella, Blast and ARG-ANNOT
type: Document
related_post:
comments: true
doi: 10.1128/AEM.00140-17
---

## Summary

|||
|----|----|
|category|assembly-based|
|platform|illumina|
|open source|true|
|reproducible|true|
|documented|true|


## Database

This protocol uses the ARG-ANNOT database as curated by the [SRST2](https://github.com/katholt/srst2). Not completely clear which file of the several ARG-ANNOT databases provided on the site that was used.


## Protocol


* Step 1 - Trimming

Trimming using trimmomatic1.32

* Step 2 - Assembly

Assembly done using SPAdes-3.0.0

* Step 3 - AMR detection

Detection using blastn-2.4.0
Criteria:  ≥50% coverage and ≥75% nucleotide identity


## Citation

The paper(s) documenting this protocol:

* Carroll _et. al._. [Whole-Genome Sequencing of Drug-Resistant Salmonella enterica Isolates from Dairy Cattle and Humans in New York and Washington States Reveals Source and Geographic Associations](https://aem.asm.org/content/83/12/e00140-17.full)
