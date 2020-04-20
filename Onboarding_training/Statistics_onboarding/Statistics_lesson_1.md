# Lesson 1 - "Getting set up"
---
# Learning objectives
* Describe R, RStudio, and Environment
* Use RStudio GUI to test basic R functionality
* Read-in data and provide basic summary information

# Tasks:
* Step 1: Download and install R/RStudio
* Step 2: Install R packages
* Step 3: Introduction to R
* Step 4: Learn how to read-in data to R and provide general information about files.

# Deliverables:
* Given a count matrix file, taxonomy file, and sample metadata file, students must read-in all data to R and submit an email with:
  * The number of rows and columns for each file
  * A short description of what kind of samples are being analyzed
  * A short description of what the taxonomy file contains and how it relates to the count table.

# Additional resources:
  * [R programming coursera course](https://www.coursera.org/learn/r-programming)
  * [Introduction to R workshop](https://bioinformatics.ca/workshops/2018-introduction-to-R/)

--- 

## Step 1 - Download and install R/Rstudio
### What is R and why do we use it?
["R"](https://www.r-project.org/about.html) is an open-source programming language that we use for analyzing microbiome and resistome count matrices.

To facilitate the use of R we recommend using the GUI software, [RStudio](https://rstudio.com/).

### Task
* Install R and R studio on your computer following [these instructions](https://www.datacamp.com/community/tutorials/installing-R-windows-mac-ubuntu).


## Step 2 - Install R packages
### Packages greatly enhance R functionality for statistical analysis
Description here
### Task
* Learn how to install R packages with the following resource (XXXX) and succesfully install all of the following packages in your environment:
  * vegan
  * ggplot2
  * etc.

## Step 3 - Introduction to R programming
### R scripts and "projects"
Description here

### Task
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


## Step 4 - Reading-in data
### Getting microbiome and resistome results into R

### Task
* Download the following three files:
  * sample_metadata.csv
  * AMR_annotations.csv
  * AMR_count_matrix.csv
* Follow instructions in the R script, (XXXX), to load all three files and calculate summary statistics for each file.
* Turn in file with results.


