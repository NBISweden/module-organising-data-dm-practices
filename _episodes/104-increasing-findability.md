---
title: Maintaining data integrity and authenticity
teaching: 10
exercises: 10
questions:
- What can we do to maintain data integrity and authenticity?
objectives:
- Incresing file findability
- File naming concepts
- The concept of tagging files with metadata 

keypoints:
- File findability is connected to the future value of research
- Meta tagging files with relevant infromation increases findability
- Avoid creating unncessary folders by use of smart folders 

---

> ## About this episode 
>A key point in data management is finding information among large sets of files and data. Knowing all your files and their contents can be a manageable method in the short term, but as files and folders increase in size and numbers and old projects are replaced with new ones, the once clear overview is obscured and finding specific information becomes harder. Applying a clear file naming convention can help circumvent the effects of time, and meta tagging files with identifiable information increases both file findability and allows organization of files without having to restructure data.

## Increasing file findability
We have already explored the concept of file naming conventions. Here we will focus on additional things we can do to increase file findability. 

## Multiple file copies
One way to increase findability is to make copies of files used in separate contexts and store these in process specific locations. For each context a new copy of a file is made and stored separately. The risks with such a procedure should be obvious to everyone. The same problem also applies to collaborations lacking common storage and working spaces. Files may be distributed among project participants using portable devices (Flash drives, hard drives, etc.), creating a situation where multiple copies exist in parallel.

Pros: Someone is guaranteed to have the latest version of a file

Cons: Who has the latest version of a file?

A system dependent on tracking the use of multiple file copies are strongly adviced against! 

## What is a meta tag?
A meta tag is an information snippet attached to a digital file in order to help organizing and find relevant assets within a group of objects. There are three main types of meta tags:

- Descriptive (Describes the asset using keywords, author, file content, etc.)
- Structural (Provides information about how the asset is organized, i.e. if it is part of one or more collections)
- Administrative (File type or date of creation)

All files today are automatically created with administrative meta tags. Most files are also pre-prepared with one or more empty text fields for additional tags. By using a combination of different tags we can virtually cluster data and information and make it searchable without having to re-organize the actual files and folders. 

## Meta tagging a file
- Mac
    - Bring up the file information window by selecting a file and pressing 'cmd+I'. Find the free text panel named 'Comments' in the window. 
    - Add meta tags as free text. Multiple tags are separated by white spaces. The OSX will index your files based on the input. 
    - Search the file in the search pane using the tag(s). 

- Windows
    - Right click a file and select 'Properties'
    - Go to the 'Details' tab, and look for 'Tags'
    - Click on the empty space next to it and type in your tags. Multiple tags are separated by semicolons ';'
    - Search the file using the search function

- General notes for Windows 10
    - Tagging multiple files at once is possible by selecting the files while pressing the 'CTRL' key, right click, and then selecting 'Properties'. Add the tags you want shared for all selected files.
    - Tags are inherited when files are converted into other file formats
    - Not all files are supported for adding tags. 


## Using meta tags to create Smart folders
An alternative to moving files between folders is to create smart folders (aka smart searches). A smart folder is not a folder per se, but a saved search appearing visually as a folder in the operating system. Opening the folder re-initiates the search and returns the result as a file list, just like a regular folder. Smart folders appear different in Windows and OSX. 

- Windows
    - 

- Mac
    - Using 'Finder', search for a file, or set of files, using tagged words
    - Click on 'Save' and select a location for the smart folder to be stored
    - The smart folder will appear as a differently colored icon at the chosen location.


## Meta tagging vs. Folder structure
A research project often require files to be stored in specific folders, reflecting a certain level of data organization. Ideally a file is only used in the folder where it is stored, but there may be several occasions when a single file is used in two contexts at once. As keeping multiple copies of the same file is advices against, two methods can be applied to circumvent the problem:

- Create shortcuts

  Rather than moving the file we create a shortcut, or link, from the folder to a file in a target directory.

  Pros: Shortcut appear as a file in the folder system. Intuitive.

  Cons: In case the original file is moved the link can break

- Create a smart folder

  In cases a project, or sub-project, share files we can create smart folders in the target directories linking to a single file location.

  Pros: No need to update shortcuts or target file locations

  Cons: Requires proper file tagging 

## Exercise - File Organization

Download the compressed file [File name] from [Download location] and unzip on your laptop. The file contains a collection of files from an imaginary project, somewhat resembling what the initial phase of a project can look like. Given the files provided:

- Create a proper hierarchical folder system based on the file names and contents
- Rename files in a consistent manner if required, such that it reflects both contents and file version 
 
- Meta tag files with keywords according to file contents
- Create a smart folder for a set of meta tagged files 





```
 10_final-figs-for-publication.R
 1_data-cleaning.R
 2_fit-model.R
```