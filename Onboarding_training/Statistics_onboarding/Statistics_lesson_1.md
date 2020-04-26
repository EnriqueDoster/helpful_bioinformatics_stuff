# Lesson 1 - "Getting set up"

## Learning objectives
* Describe R, RStudio, and Environment
* Use RStudio GUI to test basic R functionality
* Read-in data and provide basic summary information

## Tasks:
* [Step 1](#step-1-install-r-and-rstudio): Download and install R/RStudio
* Step 2: Install R packages
* Step 3: Introduction to R
* Step 4: Learn how to read-in data to R and provide general information about files.

## Deliverables:
* Given a count matrix file, taxonomy file, and sample metadata file, students must read-in all data to R and submit an email with:
  * The number of rows and columns for each file
  * A short description of what kind of samples are being analyzed
  * A short description of what the taxonomy file contains and how it relates to the count table.

## Additional resources:
  * [R programming coursera course](https://www.coursera.org/learn/r-programming)
  * [Introduction to R workshop](https://bioinformatics.ca/workshops/2018-introduction-to-R/)

--- 

# Step 1 - Install R and Rstudio
## What is R and why do we use it?
["R"](https://www.r-project.org/about.html) is an open-source programming language that we use for analyzing microbiome and resistome results. R provides a wide variety of statistical (linear and nonlinear modelling, classical statistical tests, time-series analysis, classification, clustering, …) and graphical techniques, and is highly extensible. 

To facilitate the use of R we recommend using the GUI software, [RStudio](https://rstudio.com/).

## Task
* Install R and R studio on your computer following [these instructions](https://www.datacamp.com/community/tutorials/installing-R-windows-mac-ubuntu).


# Step 2 - Install R packages
## Packages greatly enhance R functionality for statistical analysis
Description here

## Task
* Learn how to install R packages with the following resource (XXXX) and succesfully install all of the following packages in your environment:
  * vegan
  * ggplot2
  * etc.

# Step 3 - Introduction to R programming
## R scripts and "projects"
R code can be run directly in the R terminal, or can be organized in to a series of steps within an [R script](http://mercury.webster.edu/aleshunas/R_learning_infrastructure/R%20scripts.html). R scripts facilitate reproducibility as all your code can be stored in a single file and shared for others to replicate.

[RStudio projects](https://support.rstudio.com/hc/en-us/articles/200526207-Using-Projects) make it easy to organize different datasets, each with their own working directory, workspace, history, and source documents.
* During an R session, you might define a large number of R-objects: variables, data structures, functions etc., and you might load packages and scripts.
* All of this information is stored in the so-called "Workspace". When you quit R you have the option to save the Workspace; it will then be restored in your next session. Now, you might think: how convenient - I can just stop R, and when I restart it, it will go into the same state as it was. But no. Restoring the Workspace from a previous state is actually a bad idea: if you load data or variables in a startup script, they may be overwritten with a corrupted version that you happened to save in the workspace when you last quit. This is very hard to troubleshoot. Essentially, when you save and reload your Workspace habitually, you have overlapping and potentially conflicting behaviour of startup script and Workspace restore.

* Instead, we recommend the following:
  * Never save the Workspace.
  * Always work from scripts.
  * Write your scripts so that you can easily recreate all objects you need to continue your analysis.
  * If some objects are expensive to compute, you can always save() and later load() them explicitly. In fact, restoring the Workspace does the same thing, but you have less control regarding whether the version of your objects are correct, and what temporary variables may be loaded as well.
  * In this way, you work with explicit instructions, not implicit behaviour.
  * Explicit beats implicit.



## Task
* Open Rstudio and set working directory to the newly downloaded directory, "MEG_onboarding_lessons"
* Create a new R project called "Lesson 1 project" and follow the instructions in the script (XXXX) to familiarize yourself with basic R functions.
* Open RStudio.
* Select File → NewProject…
* Click on Version Control.
* Click on Git.
* Enter https://github.com/EnriqueDoster/MEG_onboarding_lessons as the Repository URL
* The project directory name should automatically fill out, or you could change it to anything else you want.
* Click on Browse… to find where you want the project to be created.
* Click Open.
* Click Create Project; the project files should be downloaded and RStudio should re-start with the new project data.
  * NB. Your working directory is now wherever you selected to download the github files. 
* Look at the bottom right panel in Rstudio to view files in your new working directory.
  * Click on the "Statistics" directory
  * Open the "Lesson1_R_introduction.R script by clicking on it.
  * Follow instructions on the script to get familiarized with R. 


# Step 4 - Reading-in data
## Getting microbiome and resistome results into R

## Task
* Download the following three files:
  * sample_metadata.csv
  * AMR_annotations.csv
  * AMR_count_matrix.csv
* Follow instructions in the R script, (XXXX), to load all three files and calculate summary statistics for each file.
* Turn in file with results.


