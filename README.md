<div class="nav">

## Goals for this repository

* First, function as a place that helps me organize the various resources I used to learn about bioinformatic anaylysis of the microbiome and resistome.
* Eventually, create useful tutorials to help others learn about bioinformatics.
  - For now, the tutorials are roughdrafts written for specific projects that I aim to improve over time.

## Contribute
Have a tool or resource that you love and think would be helpful to others? Just send a Pull Request with the details!

## Table of Contents

- [Research groups](#research-teams)
- [Important Manuscripts and Useful Resources](#important-papers)
- [Tools for your computer](#computer-tools)
- [Cheatsheets](#cheat-sheets)
- [Tutorials](#tutorials)
- [MEGARes](#megares)
- [AMR++](#amrplusplus)
  - [Pipeline overview](#pipeline-overview)
  - [QC trimming](#qc-trimming)
  - [Host filtering](#host-filtering)
  - [Resistome analysis](#resistome-analysis)
    - [Alignment to MEGARes](#alignment-megares)
    - [Filtering counts](#filtering-counts)
    - [Genes that require SNP confirmation](#snp-confirmation)
    - [Resistance Gene Identifier](#rgi)
    - [Analyzing SNPs](#analyzing-snp)
- [Statistical analysis](#stats)
  - [Overview](#stat-overview)
- [Whole-genome-sequencing](#WGS)


</div>

<main>
      
      
<article id="research-teams">
  
## Research groups


* [MEGlab](http://megares.meglab.org/) - "Our international multidisciplinary group of scientists and educators is addressing the issues of antimicrobial resistance (AMR) and microbial ecology in agriculture through research, outreach, and education. By characterizing risks related to AMR and microbial ecology, our center will identify agricultural production practices that are harmful and can be avoided, while also identifying and promoting production practices and interventions that are beneficial or do no harm to the ecosystem or public health. This will allow society to realize “sustainable intensification” of agriculture."
* [Noyes Lab](https://www.thenoyeslab.org/) - "We are a curious, driven and genuine group of individuals who unite around the common goal of scientific discovery. We cherish diversity -- of thoughts, backgrounds, experiences, skills and opinions.  We encourage (even relish!) respectful debate, and we value each others' quirks. We believe that livestock animals are an essential and valuable part of our local and global society.  We eschew the notion that livestock production is inherently at odds with human and environmental health.  And we use scientific discovery to advance livestock production in a "win-win" manner --  to benefit animals, humans and the planet. "

- Other groups with great websites

* [Huttenhower Lab](https://huttenhower.sph.harvard.edu/) - "My group includes a range of expertise on genomic data, biological network analysis, and bioinformatic methodology. We're interested both in developing new computational methods, particularly for microbial community analysis, and in applying these to the study of metagenomics, individual microbes and pathogens, and the human genome. Whenever possible, all of our studies are accompanied by tools to make the resulting methodology available to the community. Many of these goals are shared by other members of the Biological Sciences in Public Health program, the Broad Institute, and the MiRiBA consortium."

  
</article>



<article id="important-papers">
  
## Important Manuscripts and Useful Resources

- Data analysis
  * [Consistent and correctable bias in metagenomic sequencing experiments](https://elifesciences.org/articles/46923) - Important biases in metagenomic sequencing projects
  
- Writing manuscripts
  * [Science Forum: Ten common statistical mistakes to watch out for when writing or reviewing a manuscript](https://elifesciences.org/articles/48175?utm_source=Nature+Briefing) - Useful manuscript writing tips
  
- Misc. resources
  * [Micro Binfie Podcast](https://soundcloud.com/microbinfie) - New podcast focused on microbial bioinformatics
  * [Early Career Researchers](https://ecrcentral.org/) - Resources for early career scientists.
 
  
</article>






<article id="computer-tools">
  
## Tools for your computer

- Text editors
  * [Atom](https://atom.io/) - a lightweight, open-source editor featuring Teletype, a tool for real-time collaboration. 
  
- R-programming
  * [Export figure to vector](https://cran.r-project.org/web/packages/export/export.pdf) - command in R that converts R graphics (including ggplot graphics) into PPT as *vector drawings*
  * [Plotly](https://plot.ly/) - Tool for making 3D R figures
  
- Other visualization tools
  * [Tableau](https://www.tableau.com/academic/students) - Great software for creating figures using a drag-and-drop GUI.
  
  
</article>




      
<article id="cheat-sheets">
  
## Cheatsheets

* [Devhints](https://devhints.io/) - handy syntax & command reference for hundreds of languages and technologies

</article>




<article id="tutorials">
  
## Tutorials

- Ideas for presentations
  * [Pinterest Poster Design examples](https://www.pinterest.com/doipathompong/scientific-poster-design/) - "Collection of nice posters on pinterest."
- R programming tutorials
  * [Practical ggplot](https://wilkelab.org/practicalgg/) - Good tutorial for using ggplot to create a variety of figures
  * [R Graph Gallery](https://www.r-graph-gallery.com/all-graphs.html) - Gallery of various plots made in R and the code used to create them.
  * [Top 50 ggplot2 visualizations](http://r-statistics.co/Top50-Ggplot2-Visualizations-MasterList-R-Code.html) - "This is part 3 of a three part tutorial on ggplot2, an aesthetically pleasing (and very popular) graphics framework in R. This tutorial is primarily geared towards those having some basic knowledge of the R programming language and want to make complex and nice looking charts with R ggplot2."

</article>






<article id="MEGARes">

## MEGARes

* [MEGARes](http://megares.meglab.org/) - The MEGARes database contains sequence data for approximately 8,000 hand-curated antimicrobial resistance genes accompanied by an annotation structure that is optimized for use with high throughput sequencing. The acyclical annotation graph of MEGARes allows for accurate, count-based, hierarchical statistical analysis of resistance at the population level, much like microbiome analysis, and is also designed to be used as a training database for the creation of statistical classifiers.

</article>






<article id="amrplusplus">
  
## AMR++

* [AMR++ v2.0](http://megares.meglab.org/amrplusplus/latest/html/v2/index.html) - The Microbial Ecology Group's bioinformatic pipeline for microbiome and resistome analysis.

</article>






<article id="stats">
  
## Statistical analysis

* [GustaME](https://sites.google.com/site/mb3gustame/) - Great resource that provides an overview to many common statistical methods for bioinformatics.
* [Ordination overview](http://ordination.okstate.edu/overview.htm) - Overview of various ordination method with good descriptions.

</article>






<article id="WGS">
  
## Whole-genome-sequencing

- Useful papers
  * [Comparing Genomic Variant Identification Methods](https://www.biorxiv.org/content/10.1101/733642v1) - Manuscript "Genomic variant identification methods alter Mycobacterium tuberculosis transmission inference"
  * [Population structure in time-scaled phylogenies](https://www.biorxiv.org/content/10.1101/704528v1) - Identification of hidden population structure in time-scaled phylogenies

</article>










