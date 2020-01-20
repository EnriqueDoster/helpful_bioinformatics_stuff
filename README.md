<div class="nav">

## Goals for this repository

* First, function as a place that helps me organize the various resources I used to learn about bioinformatic anaylysis of the microbiome and resistome.
* Eventually, create useful tutorials to help others learn about bioinformatics.

## Contribute
Have a tool or resource that you love and think would be helpful to others? Think you could help improve any of the text in this repository's documentation?
Just send a Pull Request with the details!

##### Disclaimer: The following guide is meant as a general overview of we, the Microbial Ecology Group, does to analyze metagenomic sequencing samples. We attempt to keep up with the latest in “best practices”, but these analytic tools continue to improve and the correct combination of tools and statistical methods is in perpetual debate. Please let us know if you have any questions, require clarification, or want to help us improve our methods!

## Overview
---

* Level 1 - Core requirements for lab members
    * First step: Server log-on and navigation. 
      * Objectives: 
      * Resources:
        * Tutorial of basic commands (cd, ls, pwd, htop)
        * Videos from codeacademy or free educational account from data.camp? (could also work for R)
      * Deliverable: File that contains:
        * PATH to a kraken database
        * PATH to sequence reads
        * PATH to MEGARes
        * Find hidden file (based on hint with use of "ls")
    * Second step: Working with files
      * Objectives: 
        * Make directories/files and edit them.
        * Move, copy, remove files. 
        * Find size of directories.
        * Download files.
      * Resources:
        * Tutorial showing:
          * Make directory on "/scratch.global/"
          * Find and download a bacterial genome on local computer and use filezilla to upload to new directory on server.
          * Find the number of headers in the genome using grep (this code is provided)
          * Create file with your name and date on it.
          * Copy file and rename to something else. 
          * Dangers of RM *
      * Deliverable: Send file with:
          * PATH to created file
          * PATH to uploaded genome
* Level 2 - Running AMR++
  * First step
      * Objective: Using screen to run commands. Modules on MSI.
      * Resources: 
* Level 3 - Making custom nextflow pipelines/ running other tools
* Level 4 - 



[Acquiring sequencing data](#acquiring-sequencing-data)

[Bioinformatic analyses](#bioinformatic-analysis)

[Statistical analysis](#statistical-analysis)

* [Count normalization](#count-normalization)

* [Alpha diversity](#alpha-diversity)

* [Differential feature abundance](#differential-feature-abundance)

* [Ordination](#ordination)

* [Heatmaps](#heatmaps)


## Acquiring sequencing data
---
* Sample collection
* DNA extraction
* Library preparation
* Metagenomic sequencing
  * DNA libraries are sequenced and samples must be demultiplexed

## Bioinformatic analysis
---
* Bioinformatic analyses


## Statistical analysis
---

* Statistical analysis is undoubtedly the most complex component required for characterizing metagenomic sequencing samples. We adopt a lot of the techniques developed for ecology to analyze the multivariate data representing the microbiome and resistome. 

* We use the R programming software with various R software packages and you can see the main code we use at this repository (https://github.com/EnriqueDoster/MEG_R_metagenomic_analysis).
  * Diversity metrics and ordination : vegan
  * Count normalization and ZIG model: metagenomeSeq
  * data handling and manipulation: data.table
  * plotting : ggplot2
  * handling Qiime2 results and unifrac distances: phyloseq

### Count normalization

* The count of classified reads will first need to normalized to account for differences in sequencing performance between samples. There are many ways to normalize counts and we use “Cumulative sum scaling”(CSS) developed by Paulson et al 2013 (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4010126/).
* Then, the CSS-normalized counts are used for all the following methods of summarizing metagenomic samples (and check out this helpful website https://mb3is.megx.net/gustame/home):

### Alpha diversity

* Alpha diversity
  * Indices like “Richness”, “Shannon’s index” or "Simpson's index" to summarize the microbiome/resistome with a single value that represents the unique number of features and how evenly distributed the counts were, respectively.
* Plotting alpha diversity values with boxplots.


### Differential feature abundance

* Feature abundance in metagenomic sequencing projects
  * Comparing relative abundances is troublesome because of issues inherent to compositional data (ie. the proportion of a feature is directly affected by changes in proportion of other features) and because count tables contain many zeroes (sparse). 
      * Therefore, we use a “Zero-inflated Gaussian model” (ZIG) that allows us to combine two different distributions and fit a model that better represents metagenomic count data. Log fold changes in abundance are estimated and the Benjamini-Hochberg method is employed to adjust p-values for multiple testing.
        * Take a look at the “stats” directory and look for the file named “Group_Microbiome_Phylum_GroupNorm-GroupProb_Model_Contrasts.csv”.
         * These results have to be interpreted carefully because low abundance features will often be significantly different between sample groups. In combination with your knowledge of which features are most abundant in your samples, pick a threshold value for “Avg. Expression” and report everything above that threshold. For example, you might say something like out of 27 compared, X phyla had average expressions > 1 and X were significantly different between sample groups (p-value < 0.05).

### Ordination

* Ordination
  * Non-metric multidimensional scaling
