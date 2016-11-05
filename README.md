---
layout: lesson
title: Data carpentry -- Starting with R for data analysis
keywords: ["R", "subset", "data.frame", "read.csv"]
---

This is an introduction to R designed for participants with no programming
experience. These lessons can be taught in 3/4 of a day. They start with some
basic information about R syntax, the RStudio interface, and move through how to
import CSV files, the structure of data.frame, how to deal with factors, how to
add/remove rows and columns, and finish with how to calculate summary statistics
for each level and a very brief introduction to plotting.

(This particular set of lessons was originally revised by 
[Karl Broman](http://kbroman.org) for a
[Data Carpentry workshop](http://uw-madison-aci.github.io/2016-06-01-uwmadison/)
at UW-Madison on 1-2 June 2016.)

The current version was revised by [Laura Saba](http://www.ucdenver.edu/academics/colleges/pharmacy/Research/ResearchLabs/Systems-Genetics-and-Bioinformatics/Pages/default.aspx) for a Software Carpentry workshop at University of Colorado Denver Anschutz Medical Campus on November 5th, 2016.

> ## Prerequisites
>
> * Having RStudio installed

## Topics

* [Introduction to R](01-intro-to-R.html)
* [Aggregating and analyzing data with dplyr](02-dplyr.html)
* [Plotting data with ggplot](03-ggplot2.html)

## Other resources

* [Motivation](motivation.html)

## Organization of the repository

The lessons are written in Rmarkdown. A Makefile generates an html page for each
topic using knitr. In the process, knitr creates an intermediate markdown
file. These are removed by the Makefile to avoid clutter.

The Makefile also generates a "skeleton" file that is intended to be distributed
to the participants. This file includes some of the examples used during
teaching and the titles of the section. It provides a guide that the
participants can fill in as the lesson progresses. It also avoids typos while
typing more complex examples. Each topic generates a skeleton file, and the
files produced are then concatenated to create a single file and the
intermediate files are deleted. To be included in the skeleton file, a chunk of
code needs to have the arguments `purl=TRUE`.
