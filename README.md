# bio-data-analysis

Draft notes for a grad course in biological data analysis and best practices

## General idea

Provide first year grad students with an overview of computing concepts and tools that are frequently used in the biological sciences. 

Wide rather than deep? Expose students to many different tools they might encounter, so they know where to dig deeper when they need it. But with enough "meat" to be immediately useful -- to culture good data practices in terms of data management, data archiving, reprocucible data analysis,  skills to deal with high throughput data.


## Topic ideas

* File system organization across major OS's

* Introduction to working at the command line 

* Regular expressions -- grep 
    - example application: finding TF binding motifs

* Working with tabular data -- awk, sort, join
    - example biological application: working with GFF annotation data

* Shell scripting -- bash
    - example application: aligning reads to a reference genome

* Data wrangling in R -- dplyr and tidyr

* Visualization in R -- ggplot2

* A tour of popular biology related libraries for R

* The Python Scientific Stack -- numpy, scipy, pandas, matplotlib, jupyter notebooks

* Simulation in Python
    - example application: Boolean network modeling of a gene regulatory network 
        - [Orlando et al. 2008]() -- from Steve Haase's lab

* Working with sequence data in Python
    - example application: working with FASTA files, multiple sequence alignments, and phylogenetic trees

* Version control  -- git

* Data archiving and data management

* Introduction to databases -- sqlite
    - example biological application: building a multi-table relational database of ecological data
        * [Ames et al.](https://esajournals.onlinelibrary.wiley.com/doi/full/10.1002/ecy.1886) -- from Justin Wright's lab