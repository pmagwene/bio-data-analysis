# bio-data-analysis

Draft notes for a grad course in biological data analysis and best practices


## Summary for Dept Chair and DGS prior to Fall 2022 Retreat

We propose to develop a two-semester graduate level course, targeted at first year grad students, that will provide an overview of practical computing concepts and data anlysis tools that are frequently used in the biological sciences. In addition to developing practical skills and experience with data science, a secondary (but important) goal is socialization on new biograds into the department. 

In addition to formal coursework (a weekly 2.5 hr class session), the course will include a weekly "data lunch" where faculty, senior graduate students, and postdocs from the department will present overview of data types and data tools they use in their own research, reinforcing concepts from class and demonstrating relevance. Key goals of these data lunches are to  build community among students and students and faculty, and expose them to some of the research going on in the department.

## Text for new course request (sections follow the prompts in the request)

Expanded description: This will be a two-semester course targeted at first year graduate students in the Department of Biology. No prior programming experience is assumed. The course is designed around developing computing skills common to all areas of modern biological research. Examples in class and homework assignments will involve data generated by current graduate students in the department and will draw on the diversity of data types in the biological sciences (e.g., geospatial, images, genetic/genomic).

For reference, here is the submitted course description: This course is the first of a two-semester sequence that provides an overview of computing and data analysis concepts and tools that are frequently used throughout the biological sciences. Topics covered include: data filtering and restructuring; data visualization and effective communication; data science best practices for reproducability, reusability, and discovery; and working effectively with big data. Students will learn how to leverage key tools from the Unix, R, and Python computing ecosystems.

Course Goals and Objectives: The primary goal is to provide a foundation of practical computing concepts and skills for beginning graduate students in the Department of Biology that will aid them in their graduate resaerch and profession life well beyond. Important secondary goals are (1) inculcating best practices in data management, analysis, and dissemination, and (2) introducing each new cohort of students to more senior trainees in the department and the breadth of research they are conducting.

Course Text and Materials: The primary textbook will be "Computing Skills for Biologists" by Allesina and Wilmes (Princeton Press). Additional readings will include articles from the primary literature as well as web-based materials devoted to specific topics.  

General Course Requirements: Students will be expected to reformat, filter, sort, analyze, and visualize datasets using code they generate. This will include hands-on exercises in class as well as homework assignments. Students will also be required to attend a weekly discussion section, where more senior trainees in the department will present their reseach and discuss how they utilized computational tools to in their work. 

Assessment information: Homework assignments will be graded. Students will have the opportunity to re-submit graded assignments for an improved score, the idea being to encorage students to view code as a living document. The discussion section will be graded for attendance only. Quizzes and exams will not be used for assessment. 


## General idea

Provide first year grad students with an overview of computing concepts and tools that are frequently used in the biological sciences. Along the way, build community among students and expose them to some of the research going on in the department. And also along the way, illustrate how the material presented in class is applied to everyday research projects.

Wide rather than deep? Or generally wide, but deep in a few selected areas? Expose students to many different tools they might want to leverage, so they know where to dig deeper when they need it. But with enough "meat" to be immediately useful -- to culture good data practices in terms of data management, data archiving, reproducible data analysis, skills to deal with high throughput data. Draw on example datasets generated by biograds, illustrative of challenges/opportunities, and reflecting the diversity of research projects in the department.

Don't assume any prior programming experience. Motivate with domain-based examples. Learn from Carpentries model. 

## Possible references

General:
* [Computing Skills for Biologists: A Toolbox](https://computingskillsforbiologists.com/)

Python:


R:
* [R for Data Science](https://r4ds.had.co.nz/)
* [R Graphics Cookbook, 2nd edition](https://r-graphics.org/) 
* [Fundamentals of Data Visualization](https://clauswilke.com/dataviz/)

Unix:
* [Learn by Example: GNU Grep and Ripgrep](https://learnbyexample.github.io/learn_gnugrep_ripgrep/cover.html)
* [Learn by Example: GNU Awk](https://learnbyexample.github.io/learn_gnuawk/)

SQL:


## Structure ideas

* Weekly lecture + hands-on: 2 or 2.5-hour classroom session

* Weekly data lunches: grad students from dept present overview of data types and data tools they use in their own research; reinforcing concepts from class and demonstrating relevance; TA moderates

* Faculty talks: have a variety of faculty talk about data analysis methods, tools, reproducicibility, data archiving, and other challenges they face in their research program; then use their data sets as examples. These talks would be during normal lecture time.

* One semester or two? -- leaning towards 2 semesters to allow time for students to absorb concepts, work through homework problems 

* Integrating data visualization -- beyond the mechanics of how to make a figure, but what makes for good figure.  Drawing on Greg's current course.

## Draft high-level outline (* = more extensive modules)


0 Orientation
* Course goals and mechanics
* Working with data: clean, reformat, explore, analyze, model, present, share
* Data science principles: FAIR, open-source, non-proprietary, etc. 
* Help installing necessary software, familiarization with VSCode 

1 Unix
* First steps: intro to Unix, UNIX file system, 
* Working with remote computers/file systems: ssh, sftp, curl
* Unix basics: navigating the file system, files and directories
* Working with files: creation, viewing, comparison, permissions
* Data wrangling tools: cat, sort, uniq, tr, cut, join, wc, grep, sed, awk
* Shell Scripting
* Regular expressions: grep, sed, awk

2 R
* First steps: familiarization with R Studio environment, intro to R
* Basics: importing/exporting, base plots
* Markdown in R (or Quarto?)
* Data wrangling in R: tibbles, Tidyr, Dplyr
* Advanced data viz in R: ggplot2
* Applications for biology: geospatial and genomic data 
* Principles of effective and ethical data visualization
* Tour of useful R packages for biologists

3 Programming best practices
* It starts with the little things: commenting, variable names, choosing the right data structures, etc.
* Debugging 
* Testing and validation
* Version control: Github (using Python as an example)


4 Python
* First steps: familiarization with Jupyter (or Quarto?), intro to Python
* Basics: data structues, flow control, etc.
* Data wranging in Python: NumPy, Pandas (but not data viz and Seaborn?)
* What and how much more is appropriate here? 



5 SQL
* Relational database concepts
* Orientation to SQLite
* The all-important SELECT statement
* Deeper dive into queries: nested queries, aliases, views, joins 
* Leveraging Sql from Python and R

6 Data science best practices
* Being thoughtful: DMP
* Data integrity: secure storage, checksums, metadata, persistent identifiers
* Working with data: organizing files, file naming conventions, intermediate data products
* Choosing the right tool for the job: these and other languages
* Reproducibility throughout the workflow
* Exposing data: repositories, reusability, discoverability


### PMM Notes on sequencing:
* I've been think about how to sequence intro of material, right now I favor the following

   Unix -> R -> Python

* My reasoning is as follows:
  * Unix -- can immediately manipulate data with simple commands, introduce concepts of combining series of simple manipulations to accomplish complex tasks, emphasis on creating structured data
  * R -- most R intros assume you've already got structured data as input. Once you've got structured data can summarize, restructure, visualize, etc
  * Python -- least emphasis on structured data on input (until we get to NumPy / Pandas)


## Topic ideas: to be integrated into above structure 

* The big picture
    - data lifecycle
    - reproducibility, reusibility, discoverability
    - DMP as a living document

* File system organization across major OS's
    - interacting with remote file systems
    - transferring large files, archiving datasets

* Introduction to working at the command line 

* Regular expressions -- grep 
    - example application: finding TF binding motifs

* Data concepts
    - data and metadata
    - special data types: date, time, geolocation, etc. 
    - special values: null, NaN
    - how to deal with outliers? when is imputation appropriate?

* Working with tabular data at the command line -- awk, sort, join
    - example biological application: working with GFF annotation data

* Shell scripting -- bash
    - example application: aligning reads to a reference genome

* Data wrangling in R -- dplyr and tidyr

* Visualization in R -- ggplot2

* A tour of popular biology related libraries for R

* Introduction to Python
    - Jupyter notebooks: introduce along with starting Python?
    - example application: reorganizing and cleaning a flat file downloaded from a repository 

* The Python Scientific Stack -- numpy, scipy, pandas, matplotlib, jupyter notebooks

* Simulation in Python
    - example application: Boolean network modeling of a gene regulatory network 
        - [Orlando et al. 2008]() -- from Steve Haase's lab

* Working with sequence data in Python
    - example application: working with FASTA files, multiple sequence alignments, and phylogenetic trees

* Version control  -- git

* Data archiving and data management

* Introduction to databases -- sqlite (or postgresql?)
    - example biological application: building a multi-table relational database of ecological data
        * [Ames et al.](https://esajournals.onlinelibrary.wiley.com/doi/full/10.1002/ecy.1886) -- from Justin Wright's lab
    - sql queries
