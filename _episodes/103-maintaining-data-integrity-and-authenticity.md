---
title: Maintaining data integrity and authenticity
teaching: 10
exercises: 10
questions:
- What can we do to maintain data integrity and authenticity?
objectives:
- File naming concepts
- Conditions and use
- Data structure
- Data and structure documentation 

keypoints:
- Data integrity and authenticity is dependent on knowing what the data files contain, and who does what to what file. This requires a findable and accessible file structure, an explicit file naming concept, knowledge of whom has access to what data, and documentation of data treatment procedures. 

---

> ## About this episode 
> Scientific results are no stronger than the data they are based on, and the data strength is dependent on its integrity and authenticity. Developing good practise for maintaning data integrity and authenticity is therefore essential to guarantee high quality results.

## File structure
Any structure is better than no structure at all. Regardless of who we are we all apply, implicit or explicit, some kind of plan or structure to our data. Structure is often based on the concept of clustering, and clustering is often done either from a bottom-up or top-down perspective. 

### Bottom up
Similar or related files tend to be kept together in folders. Folders are then clustered in super folders, etc.
Example: I collect my data in a folder, and create the analysis files in the same folder. I version my data in one or more parallel folders and run more analyses there. I then create a super folder for all data/analysis folders and begin working on my manuscript there.

Pros: Easy model for everyday work, intuitive clustering inspired by workflow.

Cons: Easy to lose overview. Files may end up in "wrong" surroundings. Creates clutter. 

### Top down
Super folders are created first, then topic specific levels of sub folders. Clustering predates practise.
Example: I create an entire project folder structure, with several layers of sub folders for data, analyses, documentation etc. reflecting the project setup and workflow. When I generate data I place it in the data folder, make my analysis files in the analyses folder, and store my results in a separate folder. I begin working on my manuscript in a manuscript folder. 

Pros: Process defined file structure, follows the workflow. Ideal for third person view of project.

Cons: Rigid. Less flexible to work in with many folders, levels, and movements between folders in workflow. Files may end up (temporarily) in wrong folder due to leisure.  

In practice, we may end up with a combination of top-down and bottom-up structures. Starting with a top-down approach, we may create new sub folders based on a bottom-up work flow. Any deviance from a plan is ok, as long as we keep track on what we do and why. When time comes to end a project, knowing where to find what can save a lot of time and effort.

Working in projects where data is shared with several collaborators, a pre-defined top-down file structure may not fit any single individual perfectly, but will most likely benefit the greater good of the project most. It is a good idea to have one or two individuals responsible for overviewing and maintaining data structure in a shared project. A non-maintained file/folder structure can quickly become cluttered! 

## Etherpad exercise
Considering your own file structure, or the file structure used in your research group, write in the Etherpad: 

- If your current file structure is top-down or bottom-up, or a mix of the two. 
- Who the "inventor" of your file structure is (title, not name!), and to what extent can you influence how it is organized?
- One thing you believe you could improve in your current file structure.


## File naming
A file naming convention is a framework, or protocol, for naming your files in a way that describes the file contents and, importantly, how they relate to other files.

A well suited file naming protocol should:

- Make it easy to understand what the file is and what it contains, from just reading the file name (Human readable)
- Avoid special characters, and replace whitespace with - or _ (Machine readable)
- Include file version information when applicable
- Contain numbers and dates in ISO format

### Three principles for (file) names:

1. Machine readable – avoid spaces, deliberate punctuation, accented characters, inconsistent letter casing
2. Human readable - a name describes the content of the file, connects to concept of a *slug* from semantic URLs
3. Default ordering – put something numeric first, use the ISO 8601 standard for dates (YYYYMMDD, or YYYY-MM-DD), left pad other numbers with zeros (01, 02, 03... 10)

<!-- Yvonne suggests to add an exercise on file naming, eg give a set of alternative file names and ask which ones are 'good enough' and why (or ask them to improve the bad examples) -->

### Bulk file names:
Data producing equipment (and software) sometimes generate files with pre-defined names. These can be made up of a serial number or text string along with machine specific information. To a non-user such files may seem incomprehensible, and may require explanation in order to make sense. To preserve the third-person view of files where the file name does not provide information of content or origin, sufficient documentation is required. Use sub-folders to cluster such files in manageable numbers and add README-files for orientation and explanation (Remember your future self!).

### Bulk file name changes:
Sometimes continuous file name changes need to be done to generated data or analysis files. Manual modifications can be cumbersome and introduce typos. Consider using a bulk file name change tool to save time and prevent errors and maintain consistency.
<!-- Yvonne suggests to include examples of such tools -->

### Documentation of file structure:
Everyone knows their file system. A well documented file system where structure and hierachy is explained may seem unnecessary to many, but can be an essential tool for the longivety of the data. There are two cases where this is particularly important:

- Shared projects

  In any setting where data is shared in a research group or among colleagues, a documented file system can act as a guarantee that files are handled in a similar fashion by all involved. In situations where some individuals are more focused on data production, and others on data analysis, an explicit description of what files goes where along with file contents, may act as safeguards for data integrity and authenticity.

- Project ending

  Regardless of how many are involved in a project, at some time after it ends memory will start to fade on the specifics of file names and contents. Counting ones future self into the category of "third persons", a file structure documentation will be beneficial for when you need to go back to your data, or when someone else will reuse the data and/or results.

File structures are best explained and elaborated on in plain text README-files (plural). A good practice is to summarize the contents of folders on separate levels, trying to answer the question "What do someone else need to know about the contents of this folder in order to understand it?". Adding such knowledge will increase both data findability and reuseability.

<!-- Yvonne suggests to either give an example of what a readme-file can look like or create an exercise given a folder (or several if one wants them to create two readme's) with a set of files that are good enough named that they can deduce what they are and thus write about them -->

### Conditions and use:
Knowing who does what to what, when it happens, and why, is essential in maintaining data integrity. If not already present, consider upgrading your file structure with an explicit Conditions and use agreement, and apply it in file permissions.

<!-- Yvonne suggests to give an example of such an agreement -->