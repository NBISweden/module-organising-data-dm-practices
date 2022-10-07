---
title: Spreadsheet data
teaching: 20
exercises: 15
questions:
- What are good practices for structuring data and metadata in spreadsheets?
objectives:
- Understand what to consider when using spreadsheets in a project or working group
- Adopt good practices for structuring tabular data in spreadsheets

keypoints:
- Create a new file or tab with your cleaned or analyzed data
- Keep track of the steps you took in your clean up or analysis
- Keep your spreadsheets simple – put each observation in its own row and each variable in its own column
- Export the cleaned data to a text based format

---

[spreadsheet-setup-updated]: ../fig/tabular-data/spreadsheet-setup-updated.png
[multiple-info]: ../fig/tabular-data/multiple-info.png
[single-info]: ../fig/tabular-data/single-info.png
[2_Multiple_Tables]: ../fig/tabular-data/2_Multiple_Tables.png
[3_white_table_1]: ../fig/tabular-data/3_white_table_1.jpg
[formatting]: ../fig/tabular-data/formatting.png
[good_formatting]: ../fig/tabular-data/good_formatting.png
[5_excel_dates_1]: ../fig/tabular-data/5_excel_dates_1.jpg

> ## About this episode 
> We tend to organize data in spreadsheets as we humans want to work with the data, but computers and humans see it in different ways. In order to use tools that make computation more efficient, we need to structure our data the way that computers need it. This episode will cover:
>
> 1. TOC
> {:toc}
> {: .toc}
{: .callout .toc}

## Good practices for structuring data tables
The most common mistake made is treating spreadsheet programs like lab notebooks, i.e relying on context, colors, notes in the margin, and spatial layout of data and fields, to convey information. Humans can (usually) interpret such information, but computers view information differently. Unless we explain what everything means (and that can be hard!), a computer will not be able to see how our data fits together.

Setting up well-formatted tables early in the research process is extremely important – **before** you even start entering data. Once data is entered, even from a trial or test, we are less motivated to make changes to the format itself.

Data organization can make it easier or harder to work with data. Your future self might not agree with your present self on the best input format! 

### Early metadata
An important thing to consider is to adapt to using metadata standards early in the research phase. Adopting a metadata standard for your collected data, and sticking to it, will make later phases much easier. A dataset pre-adapted to publication will be the source of far less headache than a non-adapted. 

> ### Note
> The best layouts/formats (as well as software and
> interfaces) for **data entry** and **data analysis** might be
> different. It is important to take this into account, and ideally
> automate the conversion from one to another.
{: .callout}

### Keeping track of your analyses

When working with spreadsheets during data clean up or analyses, it is very easy to end up with a spreadsheet that looks different from what you started with. In order to be able to reproduce your analyses or figure out what you did when your team or supervisor asks for a different analysis, you **must:**

- **...create a new file or tab with your cleaned or analyzed data.**
<br>
Do not modify the original dataset, or you will never know where you started!

- **...keep track of the steps you took in your clean up or analysis.**
<br>
You should track these steps as a researcher would each step in an experiment. You can do this in another text file, or a good option is to create a new tab in your spreadsheet with your notes. This way the notes and data stay together.

This might be an example of a spreadsheet setup:

![spreadsheet setup][spreadsheet-setup-updated]

We will put these principles into practice today during the exercise.


### How to structure data tables in spreadsheets

The cardinal rules of using spreadsheet programs for data:

1. Put all your **variables in columns** - the thing you are measuring, like 'length' or 'attendance'.
2. Put each **observation in its own row**.
3. **Don't combine multiple pieces of information in one cell**. Sometimes it just seems like one thing, but think if that is the only way you want to be able to use or sort that data.
4. **Leave the original (raw) data raw** - don't mess with it!
5. Export the cleaned data to a **text based format** like CSV. This ensures that anyone can use the data (remember the *I* in *FAIR*?), and is the format required by most data repositories.

To illustrate, we will use participant data from a workshop. Different people have entered data in to a spreadsheet to keep track of things like date, number of attendees, and who
delivered the workshop.

If they were to keep track of the data like this:

![multiple-info example][multiple-info]

the problem is that attendees are split in types (post-graduate researcher (PGR), post-doctoral research associate (PDRA), and other), but retained in the same cells. If we want to look at attendance by type, it would be hard to set up the data. If instead we split attendee categories in different columns, it would be much easier.

### Columns for variables and rows for observations

The rule of thumb, when setting up a datasheet, is **columns =
variables**, **rows = observations**, **cells = data** (values).

So, instead we should have:

![single-info example][single-info]

## Tips and tricks for working with spreadsheets

Many things can happen when we enter data into a spreadsheet. Without claiming a comprehensible list, some of the things we can consider to make it easier for ourselves are: 

### Avoiding multiple tables {#tables}

A common strategy is creating multiple data tables within one
spreadsheet tab. **This confuses the computer, avoid at all cost!**. Multiple tables within one spreadsheet create
false associations between cells for the computer, which sees each
row as an observation. You are also potentially using the same field name in multiple places, which will make it harder to clean your data up into a usable form. 

The example below depicts the problem:

![Screengrab of spreadsheet showing formatting errors - multiple tables in one sheet][2_Multiple_Tables]

<br>

### Avoiding multiple tabs {#tabs}

Many tabs are good tabs, right? Well, yes and no. Creating extra tabs make the computer miss data connections that are there (which must be re-introduced using spreadsheet application-specific functions, or scripting). Say, for instance, you make a separate tab for each year.

Try to avoid it for two reasons:
* You are more likely to accidentally add inconsistencies to your data.
* You add an extra step for yourself before an analysis because you need to combine the data into a single data table. 

Your data sheet might end up being very extensive over the course of recording data, making it harder to enter data and maintaining an overview. For spreadsheets with many rows, use a Freeze Pane or Fixed Header function (do NOT repeat header rows!).

[Documentation on how to freeze column headers in Microsoft Excel](https://support.office.com/en-ca/article/Freeze-column-headings-for-easy-scrolling-57ccce0c-cf85-4725-9579-c5d13106ca6a)

[Documentation on how to freeze column headers in LibreOffice Calc](https://help.libreoffice.org/Calc/Freezing_Rows_or_Columns_as_Headers)

<br>

### Zero vs. Missing data {#zeros}

A spreadsheet cell missing data can be replaced with a zero (0), right? Zero participants at an event can be replaced by no value, because none showed up, right? 

Wrong!

To a computer, a zero is data. You measured or counted it, and it was zero. A blank cell means no measurement at all, and the computer will interpret it as a null value. Leaving zero data blank is not good in a written format, but NEVER okay when you move your data into a digital format.

<br>

### Bad null values (missing data) {#null}

How do you make explicit something that do not exist (a null value)? 

**Example**: using -999 or other numerical values (or zero).

**Solution**: To many statistical programs a numeric value can never be a null. It will depend on the final application of your data and how you intend to analyse it, but it is essential to use a clearly defined and CONSISTENT null indicator. Blanks (most applications) and NA (for R) are good choices.

From White et al, 2013, [Nine simple ways to make it easier to (re)use your data.](https://ojs.library.queensu.ca/index.php/IEE/article/view/4608) Ideas in Ecology and Evolution:

![White et al.][3_white_table_1]

<br>

### Avoid using formatting to add information  {#formatting}

**Example**: Colours! (The more the merrier). Separating data by blank rows. Merging cells to make text viewable. 

**Solution**: Simple. If you cannot add information as data in a row, move it to documentation/README. If you cannot see all text in a cell, make cell wider. Merged cells can really mess up machine readbility of data!

<br>

### Placing comments or units in cells {#units}

**Example**: You doubt the data quality of a cell and want to make a comment about it.

**Solution**: Add comments in separate cells, or in separate tab referencing the cells in question. 

<br>

### More than one kind of information in a cell {#info}

**Example**: 
You want to add linked but static data to a cell in a spreadsheet. For example, an experiement was run on mice `mus` with phenotype wrinkled skin `wrinsk`, caused by presence `+` of gene variant `Prss21`. So I can add that data in a single column as `mus_wrinsk_Prss21+`, and code data as present/absent, right? No. 

**Solution**: 
Never include more than one piece of information in a cell! Design your data sheet to include a column for each type of data. The organism is one kind of data, the phenotype a separate kind, etc. Place each one in their own column, *even if it seems unnecessary*! 

<br>

### Field name problems {#field_name}
If possible, decide on a pre-defined controlled vocabulary prior to collecting your data. Doing so will make later data publications much easier since your data is pre-adapted to the submission requirements.

For field names do not to include spaces, numbers, or special characters of any kind. Underscores (`_`) are a good alternative to spaces and consider writing names in camel-case (LikeThis.txt) to improve readability. Remember that abbreviations making sense today may not be so obvious tomorrow.

**Examples:**  

| Good Name          | Good Alternative   | Avoid                |
|--------------------+--------------------+----------------------|
| Max\_temp\_C       | MaxTemp            | Maximum Temp (°C)    |
| Precipitation\_mm  | Precipitation      | precmm               |
| Mean\_year\_growth | MeanYearGrowth     | Mean growth/year	 |
| sex                | -                  | M/F                  |
| length             | -                  | l                    |
| cell\_type         | CellType           | Cell Type            |
| Observation\_01    | first\_observation | 1st Obs              |

<br>

### Avoid special characters in data {#special}

**Example**: You treat Excel as a word processor when writing notes, even copying data directly from Word or other applications.

**Solution**: When writing longer text in a cell, avoid using things like line breaks and em-dashes. Be careful when copying data/test in from applications such as Word. Formatting and fancy non-standard characters can cause issues when exported to other software, such as appearance of sudden lines breaks. Treat all text as simple unformatted text.

<br>

### Avoid including metadata in spreadsheet {#metadata}

**Example**: You add a legend at the top or bottom of your data table explaining column meaning, units, exceptions, etc.

**Solution**: Same as before, move all explanations to a separate tab or a separate cross-referenced document.

<br>

### Using different date formats {#dates}

**Example**: You enter a full date as the value in a column. 

**Solution**: It may seem the most natural way to record dates is to write them as you say them. Spreadsheet programs have numerous “useful features” which allow them to “handle” dates, but it actually is not a good practice. Even if the spreadsheet application will display the dates in
seemingly correct way (to the human eye), how it actually handles
and stores the dates may be problematic. 

![Many formats, many ambiguities][5_excel_dates_1]

Excel **stores dates as a number** - see the last column in the above figure. Essentially, it counts the days from a default of December 31, 1899, and thus stores July 2, 2014 as  the serial number 41822.

If possible, stick to the international ISO standard date format - YYYY-MM-DD, especially if you are collaborating with colleagues used to other date formats. It will save you a lot of headache, we promise! 

<br>

> ### Exercise 9
>
> We are going to take a messy version of some data and begin cleaning it up using the information, tips and tricks listed above.
> (Remember to **create a new file** for the cleaned data, and **never modify the original (raw) data**.)
>
> 1. First [download the data](../data/training_attendance_start.xlsx)
> 1. Open up the data in a spreadsheet program (i.e. Excel).
> 1. You can see that there are two tabs. Various people have recorded training attendance statistics over 2016 and 2017 for two kind of training activities, and they have made notes and kept track of the data in their own way. Now you are being asked to evaluate the training programme, and you want to be able to run a few statistical analysis. You need to make the data more **machine readable**.
> 1. Together with the person next to you, work on the data to make it **both human readable and machine readable**. Clean up the 2016 and 2017 tabs, and see if all data can be merged in an easier way.
> 1. Think of a way to document what you have done, so that your future you understands the changes that was made. Where do you store that information?
>
>> ### Hints and Solution
>> 1. Can the data potentially be merged into a single tab?
>> 1. The colours used to mark cells are not explained. Is it useful to retain such information? 
>> 1. The diagrams are only visualisations of some of the data. They can be easily reproduced elsewhere and may mask other information. Can they be removed from the spreadsheet?
>> 1. It seems the attendee data is entered in a non-compatible way across the different tabs. Is there a risk of information loss, or can you merge data using a smallest common denominator approach?
>> 1. Would you store documentation of changes within or outside of the spreadsheet? Why and how?
>> 1. A suggestion on how the data can be cleaned and organised [can be downloaded here](.../data/training_attendance_end.xlsx) 
> {: .solution}
{: .challenge}


> ### Further reading
> - [Hadley Wickham (2014) Tidy Data. In Journal of Statistical Software. Vol. 59, Issue 10.](http://www.jstatsoft.org/v59/i10)
> - [ELIXIR (2021) Metadata management. In Research Data Management Kit. A deliverable from the EU-funded ELIXIR-CONVERGE project (grant agreement 871075).](https://rdmkit.elixir-europe.org/metadata_management.html)
>
{: .callout}