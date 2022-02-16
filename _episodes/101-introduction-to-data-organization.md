---
title: Introduction to data organization
teaching: 20
exercises: 10
questions:
- What are our data, and how do we keep it in order?

objectives:
- Understand what to consider for maintaining data organization strategies in a project
- Develop good practices for data storage, processing and documentation

keypoints:
- Good data organization is fundamental to any research project

---

[//]: # "[Provenance]: ../fig/storage/Provenance.jpg"
[//]: # "[life-cycle]: ../fig/storage/life-cycle.png"

> ## About this episode 
> The data that you collect, organise, prepare, and analyse to answer your research questions, and the documentation describing it, is the lifeblood of your research. However, doing so without a prior idea of structure and how data will be used or viewed in the future, by yourself or someone else, can cause the data to become difficult to understand, or even useless. Also, any working structure will tend to accumulate deviances over time regardless of initial intentions. In this episode we will look at data organization from a data life cycle perspective. 

> 1. TOC
> {:toc}
> {: .toc}
{: .callout .toc}


## The data life cycle

When we consider aspects of data organization, we can, as scientists, benefit from making our decisions based on a general data lifecycle.

[//]: # "[life-cycle]: ../fig/storage/life-cycle.png"

Throughout its lifecycle, data can, and will, be subejct to many possible types of changes:

- Data cleaning procedures may be implemented;
- Errors are often found and corrected;
- New variables may be constructed;
- New information may be added from external sources;
- File formats may be changed;
- New data may be included;
- The data file structure may be changed for the purpose of increasing operability, etc.

There are also possible types of changes to the data structure itself:

- New sub-projects can be initiated, or data splits may occur;
- Data files may be re-structured and/or re-organized into new folders;
- Collaborations can require certain data, but not all, to be stored in separate locations.


## Overview of data

Generation, processing and analysis of data inevitably result in a number of edits in the data files and file structure. However, it is necessary to preserve the authenticity of the original research information contained in the data throughout the entire data lifecycle, while trying to maintain the file structure as it was intended. To develop a strategy for data management in a project you need to combine the project plan with an overview of the data and documents your research will generate, preferably already at the startup phase. Such a list can consist of, but not be limited to:

- Data file types
- Average (and maximum) file sizes
- Initial and/or intended folder structure
- Documentation procedures

Preparing your project for receiving data should be a core aim in your research management. 

Sometimes a project will increase in size and scope, sub-projects will form, and data production will expand as new data are required and generated. When this happens, it may require changes and adaptations to already existing file structures. A file structure should be treated as a living document, continuously adapting to changes. A file structure is not decided once, and then remaining in a static state throughout the data life cycle.  


## The third-person view

When settling for a data and file structure we need to take into account more than our own personal preferences. The ultimate goal for research data is making it useful for the scientific society of today and tomorrow. Data can, and will, be important to more researchers than ourselves, and should therefore be prepared and treated in such a way that it can be read and interpreted by others. This may come in conflict with our everyday use of the data. The data and file structure we find most convenient for ourselves, here, today, may not be the most convenient structure for our future selves, or other researchers in general.

Maintaining a file system adaptable to our own changing research requirements, while also being understandable for other researchers tomorrow, can be a challenging task. We need to consider the present as well as tomorrow, and our own view as well as others.


### Preserving data timelines

As data is created and used in different analyses, it tends to split in different versions. Reasons may include modifying the contents of files, adding and/or substracting data, or creating versions for trying different kinds of analyses or analysis setups. Versions tend to accumulate over time, and without an explicit strategy may eventually make file structure overview difficult or even impossible. We can take measures to decrease such disorder:

- A coherent file naming strategy. 

    By avoiding non-hierachical file names (file.txt, file_new.txt, file_newer.txt, file_try.txt, file_add.txt etc.) we can circumvent having to re-interpret file chronology in the future. This is of particular importance when we publish data. There should never be confusion over which file was the published version. One way to prevent this is to adapt versioning of files.

- File versioning.

    An easy-to-track and widely used way to document file history is to do file versioning (file_1.0.txt, file_1.1.txt, file.2.0.txt, etc.), where each new version of the file receives a new version number. Coupled with a separate document, or registration system, where each version is explained, anyone will be able to track changes through time.


>> ### Examples of practices
>> Some best practice rules (UK Data Service, 2017a; Krejčí, 2014) can be summarised as follows:
>> - Establish the terms and conditions of data use and make them known to team members and other users;
>> - Create a ‘master file’ and take measures to preserve its authenticity, i.e. place it in an adequate location and define access rights and responsibilities – who is authorised to make what kind of changes;
>> - Distinguish between versions shared by researchers and working versions of individuals;
>> - Decide how many versions of a file to keep, which versions to keep (e.g. major versions rather than minor versions (keep version 02-00 but not 02-01)), for how long and how to organise versions;
>> - Introduce clear and systematic naming of data file versions and editions;
>> - Record relationships between items where needed, for example between code and the data file it is run against, between data file and related documentation or metadata or between multiple files;
>> - Document which changes were made in any version;
>> - Keep original (raw) versions of data files, or keep documentation that allows the reconstruction of original files;
>> - Track the location of files if they are stored in a variety of locations;
>> - Regularly synchronise files in different locations, such as using MS SyncToy (2016).
> {: .solution}
{: .discussion}


#
{: .callout}

{% include links.md %}