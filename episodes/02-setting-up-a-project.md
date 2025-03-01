---
title: 'Working with QualCoder Projects'
teaching: 15
exercises: 10
---

::: questions
-   How can documents and projects be imported into QualCoder?
-   What are the advantages of importing a QDPX project over only
    importing documents?
-   What are the key sections of the QualCoder interface?
:::

::: objectives
-   Create a QualCoder project by importing a QDPX project
-   Practice importing and organizing documents
-   Apply consistent naming conventions to project documents
:::

Once we have a general sense of the data we'll be using and what format
it needs to be in, the next step is generally to create a project in a
qualitative software package and import the de-identified raw data.

[QualCoder](https://qualcoder.wordpress.com/) is an open-source and
cross-platform tool for coding and analysis of textual data. It is
capable of working with a variety of data formats and has tools for both
qualitative and mixed methods analysis.

::: spoiler
### Qualitative software

Qualitative software is sometimes called **CAQDAS**, an acronym for
*Coding and Qualitative Data Analysis Software* to recognize the two
essential functions of qualitative research software:

1.  Apply codes or tags systematically to a collection of data sources
2.  Analyze codes (and sometimes raw data or secondary sources) to draw
    conclusions

CAQDAS have various features that may be useful for particular types of
data or methodologies. This lesson includes an [alternative software
options page](../learners/alternative-software-options.html) for those
interested in learning about other CAQDAS.
:::

## Starting QualCoder

If you haven't already installed QualCoder, please follow the
instructions in [Summary and Setup][../index.html] before proceeding.

When you first open QualCoder, it will display the `Action Log` tab with
some information about project settings and any currently-open projects,
like the example below.

![](fig/qualcoder-launch-screen.png){alt="Image of the Action Log tab of QualCoder immediately after the program is launched"}

## Creating a project

Work in QualCoder is organized in projects, each of which contain their
own sets of *files*, *codes* and other information. Click
`Project - Create New Project` and, after choosing a location where you
can easily find it later (like your `Desktop`) give the project a clear
name like `Social_media_privacy_project_planning`. This creates a new
folder whose name ends in `.qda` so QualCoder can identify it easily as
a project.

Clicking `Save` returns us to the action log, which now displays a
summary of the new project.

## Importing and navigating documents

Documents can be imported one at a time with the `Manage - Manage Files`
command. Add the `BSR_Interview_Guide` and `BSR01_Transcript` by
clicking on the `Page` icon with a `+` or pressing `CTRL+2` (Windows) or
`CMD+2` (Mac). You can select multiple files by holding `CTRL` or `CMD`
while clicking file names before clicking `Open` once you have chosen
your files.

Once the documents are imported, view the interview guide by
double-clicking its name.

::: spoiler
## PDFs in QualCoder

QualCoder converts all text and PDF documents to plain text when
importing, which removes formatting and visual elements. The
[QualCoder](https://github.com/ccbogel/QualCoder/wiki/3.2.-Files) Wiki
provides guidance on how to pre-convert PDFs to a text format if you
experience readability problems.
:::

Semi-structured interview guides often include both main questions like
**Did you publish any of the data from your example?** and planned
follow-up probes meant for when the participant doesn't volunteer as
much information as the interviewer is seeking. For the question above,
there are three probes to learn more about data publication (about 1/2
of the way down the document):

1.  Is the data published in a repository? Which one?
2.  What are your plans for storing, retaining, and deleting data in the
    future?
3.  Who has access to the data?

When finished, use `Cancel` (or `ESC`) to return to the file manager
view.

::::: challenge
### Adding documents and attributes

1.  On your own, find and add each of the `Big Social Research`
    interview transcripts from the Mannheimer project. Make sure to use
    short, clear, consistently structured names to make it easy to
    navigate between documents. Also add the BSR Interview Guide as a
    reference, though we won't add highlights because it only contains
    the questions.
2.  *(optional)* You can add attributes to files in your project, used
    to filter files or analyze coding. Use the `Add attribute` button to
    create an attribute for `Type` and click in the new field of the
    table to label each file as `BSR` (Big Social Research transcript)
    or `DOC` (supporting document). Try to filter the view to only show
    transcripts, then remove the filter so all files are visible again.

::: hint
This project already uses a sequence of numbers to distinguish
respondents without using names. One simple naming convention is
`BSR_##`, where number is the respondent number (i.e. `BSR_01`). Some
interview numbers may be missing; the readme file states why: "Two
participants declined to have their data shared."
:::

::: hint
Filtering and unfiltering rows can be performed from the right-click
context menu on a selected column.
:::
:::::

Documents can also be created and edited in QualCoder, but it's
interface is not optimized for significant edits. In general, any
changes, including the removal of [personally identifiable
information](https://en.wikipedia.org/wiki/Personal_data) from data that
will be shared, should take place before they are added to the project.

## Importing REFI-QDA Projects

In the past, qualitative data was rarely shared or reused beyond the
original study team, but two factors make it easier than ever before to
reuse qualitative data. First, repositories like QDR are helping
normalize the sharing of qualitative data to reuse for research,
transparency, and teaching. Second, a new data standard called
[REFI-QDA][<https://www.qdasoftware.org/>] was introduced in 2019 that
allows analysis projects created in one software package to be reused,
even by users with different software. REFI-QDA projects allow sharing
not just raw data, but codes, coded text, and even certain analytic
outputs.

::: spoiler
## REFI-QDA Technical Overview

REFI-QDA projects are saved as compressed folders with either a `QDPX`
or `ZIP` extension, depending on export software. They contain both the
project's raw data files and `XML` files with a custom schema including
sources, segments, codes, annotations, memos, links, cases, sets, and
sometimes visual representations of linked entities, as well as user
information (used to distinguish multiple coders on one project, for
example). Two sets of standards were developed, one for sharing only the
codebook for a project, and one for sharing the entire project.

Not all software that supports REFI-QDA includes all parts of the
standard, but because the standard was designed in collaboration with
almost all major CAQDAS software developers, it is a major step toward
an open interoperability standard. And because XML is an uncompiled text
data format, QDPX projects can even be accessed in other software (such
as R or Python) by developers familiar with the standard.

QualCoder is (as of 2025) the only free CAQDAS which supports both
codebook and project import and export using REFI-QDA.
:::

To import a REFI-QDA project to QualCoder, use `Project-Import-?????`
and select `Mannheimer_Redacted_Interivew_Analysis.qdpx` from the data
directory. After a brief time, you may see a warning about features that
are not fully implemented yet, then your action log should display
something like the following:

```
Reading from: /Users/username/Downloads/mannheimer_data_reuse/Mannheimer_Redacted_Interview_Analysis.qdpx
Creating temporary directory: /Users/username/Downloads/mannheimer_data_reuse/Mannheimer_Redacted_Interview_Analysis.\_temporary
Project XML parsing successful: True
Parse users. Loaded: 1 
Parse codes and categories. Loaded: 284
Parsed cases for file variables. Loaded: 0
Parsing sources. Loaded: 30
/Users/username/Downloads/mannheimer_data_reuse/Mannheimer_Redacted_Interview_Analysis.qdpx
loaded.

Project summary 
Date time now: 2025-03-01 16:50
mannheimer_refi_qda_project.qda
Project path: /Users/username/Desktop/mannheimer_refi_qda_project.qda
Project date: 2025-03-01 16:47:05
Files: 30. Text files: 30. Image files: 0. AV files: 0
Cases: 0
Code categories: 54
Codes: 230
Attributes: 0
Journals: 0
```

If you click the `Manage` and `Coding` tabs, you can see the sources and codes that were imported. We'll take a closer look at the codes and coded text segments in the next part of the workshop.

::: keypoints
-   QualCoder's interface has sections for managing various aspects of
    projects and uses a mix of icons, menus, and pop-up windows to
    perform actions
-   Documents should be cleaned and anonymized, if needed, before adding
    to a project
-   Consistent document naming conventions make projects easier to
    navigate
:::
