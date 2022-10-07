---
title: "Organising files and folders"
teaching: 20
exercises: 10
questions:
- What are good practices for organising files and documentation to support your project?
objectives:
- Understand what impact file organisation can have on a project or working group
- Adopt good practices for naming and organising files
- Design naming conventions for a project or working group

keypoints:
- Organisation is a key aspect of data management and will help keep the project on track by saving time and minimising risk 
- Think hard at the beginning of your project about how you are going to organise your data as it grows
- Structure project folders hierarchically to divide data into categories that can easily be understood and described
- Consider what makes sense for your project and research team, and how people new to the project might look for data files and documentation

---

[//]: # (Figures used in this document)
[files_messy_tidy]: ../fig/files-and-folders/files_messy_tidy.png
[hierarchy]: ../fig/files-and-folders/hierarchy.png
[data1]: ../fig/files-and-folders/data1.png
[data2]: ../fig/files-and-folders/data2.png
[data3]: ../fig/files-and-folders/data3.png
[slide_attribute2]: ../fig/files-and-folders/slide_attribute2.png
[slide_attribute3]: ../fig/files-and-folders/slide_attribute3.png
[slide_files]: ../fig/files-and-folders/slide_files.png
[slide_docs2]: ../fig/files-and-folders/slide_docs2.png
[slide_ex1]: ../fig/files-and-folders/slide_ex1.png
[slide_ex2]: ../fig/files-and-folders/slide_ex2.png
[slide_ex3]: ../fig/files-and-folders/slide_ex3.png
[slide_ex4]: ../fig/files-and-folders/slide_ex4.png
[awesome_names]: ../fig/files-and-folders/awesome_names.png
[plasmid_names]: ../fig/files-and-folders/plasmid_names.png
[plasmid_mac_os_search]: ../fig/files-and-folders/plasmid_mac_os_search.png
[plasmid_regex]: ../fig/files-and-folders/plasmid_regex.png
[plasmid_delimiters]: ../fig/files-and-folders/plasmid_delimiters.png
[plasmid_delimiters_code]: ../fig/files-and-folders/plasmid_delimiters_code.png
[human_readable_not_options]: ../fig/files-and-folders/human_readable_not_options.png
[slug_filenames]: ../fig/files-and-folders/slug_filenames.png
[chronological_order]: ../fig/files-and-folders/chronological_order.png
[logical_order]: ../fig/files-and-folders/logical_order.png
[chronological_order]: ../fig/files-and-folders/chronological_order.png
[logical_order]: ../fig/files-and-folders/logical_order.png
[mona_lisa]: ../fig/files-and-folders/Mona_Lisa_naming.jpg
[file_organisation]: ../fig/files-and-folders/file_organisation.png

> ## About this episode 
> This episode addresses some of the reasons to why file organisation is important for data management and a selection of good practices for organising research folders and files. The aim is to get you started and thinking about what will work for you and your project or team. Depending on your research area and the type of research you're involved in; you may find a more optimal way to organize your work.
>
> * TOC
> {:toc}
> {: .toc}
{: .callout .toc}

![Mona_Lisa_naming][mona_lisa]
<!-- https://www.instagram.com/p/CQZl6NlBdHz/ Copyright David Owens -->
## Good practices for organising files and folders
Depending on your background and experiences you could be thinking of different reasons to why it would be beneficial or useful to systematically organise your research and data files. The following is a selection of common reasons:

* Easier to locate a file
* Find similar files together
* Moving files becomes much easier
* Easy to identify which files you want to back up
* Keep organised in the long-run
* Increases productivity
* Helps you to keep and maintain a record of the project
* Projects can easily be understood by others (including your future self)

It is natural for some of your files to become unorganised from time to time, (e.g. downloads or desktop folder), and in those cases there may be multiple copies and versions of files making it challenging to find what you are looking for. You can avoid this clutter by organising your files ahead of time, and any system is better than none.

![Unorganised files on desktop][files_messy_tidy]

In this context we will be looking into practices for classifying and structuring files and folders to make them more useful. Your guiding principle should be that someone unfamiliar with your project should be able to look at your files and understand, in detail, what you did and why. This someone could be a researcher who wants to reproduce the results in your article, a new collaborator who needs to understand the details of your experiments, or more commonly, that someone could be your future self not remembering why you created a particular set of files. Poor organisation practices can lead to significantly slower research progress and you may end up having to spend significant time re-orienting yourself among files and contents you once knew.

## File and folder naming 

Names for files and folders should be consistent and meaningful to yourself and collaborators, allow for easy tracking/searching, and be somewhat descriptive of content.

An example:

`LD_phyA_off_t04_2020-08-12_norm.xlsx`

Based on the name, the file could contain information about:

* `LD` - Long day sampling, of the
* `phyA` - Phytochrome A genotype, in a 
* `off` - Medium without sucrose, at
* `t04` - Time point 4,
* `2020-08-12` - Sampled on Aug 12th, 2020, with
* `norm` - Normalised data

However, this is not obvious from the text and letters alone. Some sort of explanation is usually required, which could be added to a README-file stored in proximity to the data files.

> ### Exercise 6 - Naming and Sorting
> The following example contain files from an imaginary project, similar to the above example. To facilitate the exercise, the file name convention states that:
> - *phyA/phyB* are genotypes
> - *sXX* is the sample number
> - *LD/SD* are light conditions (Long Day, Short Day)
> - *on/off* are different growth media (on sucrose, off sucrose)
> - *date format* is the sample date
> - *tXX* is the sample timepoint 
> - *raw*, *norm* indicates raw or normalised data
>
---
```
2020-07-14_s12_phyB_on_SD_t04.raw.xlsx  
2020-07-14_s1_phyA_on_LD_t05.raw.xlsx  
2020-07-14_s2_phyB_on_SD_t11.raw.xlsx  
2020-08-12_s03_phyA_on_LD_t03.raw.xlsx  
2020-08-12_s12_phyB_on_LD_t01.raw.xlsx  
2020-08-13_s01_phyB_on_SD_t02.raw.xlsx  
2020-7-12_s2_phyB_on_SD_t01.raw.xlsx  
AUG-13_phyB_on_LD_s1_t11.raw.xlsx  
JUL-31_phyB_on_LD_s1_t03.raw.xlsx  
LD_phyA_off_t04_2020-08-12.norm.xlsx  
LD_phyA_on_t04_2020-07-14.norm.xlsx  
LD_phyB_off_t04_2020-08-12.norm.xlsx  
LD_phyB_on_t04_2020-07-14.norm.xlsx  
SD_phyB_off_t04_2020-08-13.norm.xlsx  
SD_phyB_on_t04_2020-07-12.norm.xlsx  
SD_phya_off_t04_2020-08-13.norm.xlsx  
SD_phya_ons_t04_2020-07-12.norm.xlsx  
ld_phyA_ons_t04_2020-08-12.norm.xlsx
```
---
> Try to answer the following questions:
> - Should dates be put first, and if not, why?
> - What is the difference between using leading 0 (zero) and not?
> - Is there a difference between using upper and lower case letters?
> - What is the difference between using two letters for *on* compared to three letters *ons*?
> - What are the effects if we, as in the above example, mix naming conventions?
>> ### Solutions
>>> * Using dates as leading information in file names makes finding data quickly harder as the more interesting information may be samples or timepoints (unless date is crucial to data). 
>>> * Wihtout leading zeros, sorting will make 10 and 11 appear before 2.
>>> * Upper and lower cases may sort differently 
>>> * Comparing files is easier if the file name lenghts are uniform.  
>>> * Mixed naming conventions can make it difficult to locate particular files, and/or sort a large number of files. 
>> {: .solution}
{: .discussion}


### Choose a file naming strategy
Two starting points for your file naming strategy are:

- #### A file name is a principal identifier of a file
    Good file names contain useful clues to the content, status and version of a file, uniquely identify a file and help in classifying and sorting files. File names that reflect the file content also facilitate searching and discovering files. In collaborative research, it is essential to keep track of changes and edits to files via the file name.
- #### File naming strategy should be consistent in time and among different people
    In both quantitative and qualitative research, file naming should be systematic and consistent across all files in the study. A group of cooperating researchers should follow the same file naming strategy and file names should be independent of the location of the file on a computer.


### Naming files and folders

A File Naming Convention is a framework, or protocol if you like, for naming your files in a way that describes what the files contain and, importantly, how they relate to other files. 

<br>

> ### Exercise 7
> What are examples of potential benefits of agreeing on a File Naming Convention for a project?
>
>> ### Potential benefits of a File Naming Convention
>> - Easier to process - Team members will not have to over think the file naming process
>> - Easier to facilitate access, retrieval and storage of files
>> - Easier to browse through files, saving time and effort
>> - Harder to lose!
>> - Having logical and known naming conventions in place can also help you with version control.
>> - Check for obsolete or duplicate records
> {: .solution}
{: .discussion}

<br>

## Information vs. Name length
Long file and folder names are always good because they contain more information, right? Wrong! Long names do hold more information, but also make them cumbersome. Certain software have hard coded limitations on path lengths, e.g. since Windows95 the Windows OS usually have problems with combined path lenghts exceeding 260 characters. And even in case your OS supports longer paths, some software may not. Truncated folder or file names may seriously impact findability and sortability, or even cause errors. As a problem, this also increases with folder naming and file system depth. 

### Three principles for (file) names:

1. Machine readable – Avoid spaces, deliberate punctuation, no accented characters, consistent letter casing
1. Human readable - A name describes the content of the file
1. Plays well with default ordering – put something numeric first, use the ISO 8601 standard for dates, left pad other numbers with zeros

### Do's:

* For dates use the YYYY-MM-DD standard and place at the end of the file UNLESS you need to organize your files chronologically

* Include version number (if applicable), use leading zeroes (i.e.: v005 instead of v5).
make sure the end-letter file format extension is present at the end of the name (e.g. .doc, .xls, .mov, .tif)

* Add a README.md (or PROJECT_STRUCTURE.md) file in your top directory which details your naming convention, directory structure and abbreviations


### Avoid (Don'ts):

* Using spaces (use _ or - instead)

* Dots, commas and special characters (e.g. ~ ! @ # $ % ^ & * ( ) ` ; < > ? , [ ] { } ‘ “)

* Using language specific characters (e.g óężé), unfortunately they still cause problems with most software or between operating systems (OS)

* Long names

* Repetition, e.g if directory name is Electron_Microscopy_Images, and file ELN_MI_IMG_20200101.img then ELN_MI_IMG is redundant

* Deep paths with long names (i.e. deeply nested folders with long names), as archiving or moving between OS may fail

<br>
Examples:

| Bad                                                 | Better |
| ---- |---|
| myabstract.docx                                     | 2014-06-08_abstract-for-sla.docx |
| Joe’s Filenames Use Spaces and Punctuation.xlsx     | joes-filenames-are-getting-better.xlsx |
| figure 1.png                                        | fig01_scatterplot-talk-length-vs-interest.png |
| fig 2.png                                           | fig02_histogram-talk-attendance.png |
| JW7d^(2sl@deletethisandyourcareerisoverWx2*.txt     | 1986-01-28_raw-data-from-challenger-o-rings.txt |

<br>

## How to organise files and folders
Spend some time planning how you are going to organise your data at the beginning of a project. Consider how you and others will look for and access the files throughout the project’s life cycle and ensure that all people involved can commit to using the folder hierarchy, file naming conventions, and a strategy for onboarding new contributors. You can start small and expand as you develop your practices.

### Use folders to divide files into categories
Put each project in its own folder named after that project. Ideally you want to keep the folder’s name under 32 characters long while at the same time including a combination of the project title, a unique identifier and the date. 

Consider the best hierarchy for the files in the project and decide whether a deep or shallow hierarchy is preferable. If you have several independent data collections, it is advisable to create a separate data folder for each collection. But you can use any meaningful characteristic or file attribute as a basis for organising your files, which of them will be most helpful varies widely across domains and specific projects. 
<br>
<br>
![data][slide_files]
<br>

### Folder organisation
Consider the following four different folder structures.

![file_organisation][file_organisation]

The first two (**A** and **B**) are recommended for computing.
The other two (**C** and **D**) are recommended for wet lab or biological projects.

> ### Exercise 8
> * Which one is the most similar one to your own project structure?
> * When/why would you use **A** compared to **B**?
> * When/why would you use **C** compared to **D**? 
>
>> ### Solution
>> - **A** could be preferred when you analyse different data under one unifying research question, while **B** could be preferred when you need/want to break down the data and analysis into separate variables.
>> - **C** is preferred when you organise data (in this case digital images from scans) by research object (e.g. pigs aka "patients"), while **D** is preferred when the focus of interest is an outcome of a treatment rather than the individuals themselves. 
> {: .solution}
{: .discussion}


> ### Create your own File Naming Convention 
> [Briney, Kristin A. (2020) File Naming Convention Worksheet. [Teaching Resource] (Unpublished)](https://resolver.caltech.edu/CaltechAUTHORS:20200601-161923247)
> 1. What group of files will this naming convention cover?
> 1. What information (metadata) is important about these files and makes each file distinct?
> 1. Do you need to abbreviate any of the metadata or encode it?
> 1. What is the order for the metadata in the file name?
> 1. What characters will you use to separate each piece of metadata in the file name?
> 1. Will you need to track different versions of each file?
> 1. Write down your naming convention pattern
> 1. Document this convention in a README.md (or save this worksheet) and keep it with your files
{: .callout}

> ### Further reading
>
> - [ELIXIR (2021) Data organisation. In Research Data Management Kit. A deliverable from the EU-funded ELIXIR-CONVERGE project (grant agreement 871075).](https://rdmkit.elixir-europe.org/data_organisation.html)
> - [Briney, Kristin A. (2020) File Naming Convention Worksheet. [Teaching Resource] (Unpublished)](https://resolver.caltech.edu/CaltechAUTHORS:20200601-161923247)
>
{: .callout}