# Lesson 1 - "Getting set up"
---
Learning objectives
* Describe R, RStudio, and Environment
* Use RStudio GUI to test basic R functionality
* Read-in data and provide basic summary information

Tasks:
* Step 1: Download and install R/RStudio
* Step 2: Install R packages
* Step 3: Introduction to R
* Step 4: Learn how to read-in data to R and provide general information about files.

Deliverables:
* Given a count matrix file, taxonomy file, and sample metadata file, students must read-in all data to R and submit an email with:
  * The number of rows and columns for each file
  * A short description of what kind of samples are being analyzed
  * A short description of what the taxonomy file contains and how it relates to the count table.

Additional resources:
  * [R programming coursera course](https://www.coursera.org/learn/r-programming)
  * [Introduction to R workshop](https://bioinformatics.ca/workshops/2018-introduction-to-R/)

# Step 1 - Download and install R/Rstudio
---
## What is R and why do we use it?
["R"](https://www.r-project.org/about.html) is an open-source programming language that we use for analyzing microbiome and resistome count matrices.

To facilitate the use of R we recommend using the GUI software, [RStudio](https://rstudio.com/).

## Task
* Install R and R studio on your computer following [these instructions](https://www.datacamp.com/community/tutorials/installing-R-windows-mac-ubuntu).


# Step 2 - Install R packages
---
## Packages greatly enhance R functionality for statistical analysis
Description here
## Task
* Learn how to install R packages with the following resource (XXXX) and succesfully install all of the following packages in your environment:
  * vegan
  * ggplot2
  * etc.

# Step 3 - Introduction to R programming
---
## R scripts and "projects"
Description here
## Task
* [Download this github repository](https://github.com/EnriqueDoster/MEG_onboarding_lessons)
* Open Rstudio and set working directory to the newly downloaded directory, "MEG_onboarding_lessons"
* Create a new R project called "Lesson 1 project" and follow the instructions in the script (XXXX) to familiarize yourself with basic R functions.


# Step 4 - Reading-in data
## Getting microbiome and resistome results into R
---
## Task
* Download the following three files:
  * sample_metadata.csv
  * AMR_annotations.csv
  * AMR_count_matrix.csv
* Follow instructions in the R script, (XXXX), to load all three files and calculate summary statistics for each file.
* Turn in file with results.


