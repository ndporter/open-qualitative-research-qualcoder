---
title: 'Saving and Sharing Qualitative Data'
teaching: 30
exercises: 30
---

::: questions

-   How can QualCoder projects be shared or archived in common data formats?
-   What are the advantages of sharing qualitative data?
-   What can I do to continue learning?

:::

::: objectives

-   Recognize reasons to consider archiving or sharing qualitative data
-   Practice import/export of various parts of QualCoder projects

:::

Many qualitative researchers prefer not to share or archive their data and analysis. In large part, this is because of the amount of interpretive labor they invest, along with frequent direct trusted connections with groups and individuals being studied. This trust can take time to develop before and during data collection, whether as participants or observers.

There are important advantages to archiving and sharing data, however, even for qualitative data. Each researcher ultimately must make their own decisions, but this final section will outline potential values and risks of archiving or sharing data, as well as how to go about doing so in QualCoder.

::: callout

Data sharing and interchangeable data formats have only recently become somewhat widespread in qualitative research. Be aware that information in this section may rapidly become out of date, and if in doubt, consult with a human subjects protection board, archivist, or librarian at your institution or the [Qualitative Data Repository][qdr] before sharing data.

## Import and export in QualCoder

QualCoder projects are automatically saved to your local computer as you make changes to them.We previously used the `REFI-QDA Project import` functionality (in the `Project - Import` menu) to import Dr. Mannheimer's analyzed project.

To share a project with another QualCoder user only requires copying the directory you set up when you created the project. To share with users of other CAQDAS, however, you need to export the project with the `Project - Export - REFI-QDA Project export` dialog. Choose an option on the warning screen; if you're not sure, choose the default option. Choose or create a directory for the project and click `Open`. This will create a file ending in `QDPX`.

`QDPX` files use the [`REFI-QDA Project` standard](https://www.qdasoftware.org/project), an XML-based archive format that stores both source files and core components of qualitative projects in a way that most major CAQDAS packages can recognize and import. The components that can be included are below (* indicates a feature is not fully supported in imports/exports as of QualCoder 3.6).

- sources (text, PDF, image and multimedia formats)*
- segments (specified chunks of materials/data identified as meaningful by the user)
- codes (labelled ‘tags’ attached to segments)
- annotations (comments attached to segments, codes, sources or links)
- memos (writing spaces for analytical notes, either standalone or attached to sources and/or codes)
- links between codes, segments or memos
- cases
- sets/groups of entities*
- visual representations of linked entities in the project*
- user information

You can also export only the codebook (`REFI-QDA Codebook export`) if you only want to share the names of codes and structure of the coding tree. This can be used by researchers with similar data to create a parallel coding structure, without the potential risks of sharing raw data. Codebook export files end in `QDC` instead of `QDPX`.

For more information on imports and exports, see the [QualCoder Manual](https://github.com/ccbogel/QualCoder/wiki/6.1.-Imports-and-Exports).

::: callout

### Other qualitative data formats

Each major CAQDAS package has its own proprietary data format, specialized to its features. In most cases, projects cannot be moved between software in these formats, although QualCoder does provide direct import for [`RQDA`](http://rqda.r-forge.r-project.org/) data. Data files in some software may also be restricted to specific platforms (Windows or Mac) or software versions. In general, we recommend keeping a copy of your final project in both the original format and in `QDPX` format.

:::

## Data sharing for collaboration

Working with collaborators is one of the most common reasons for sharing qualitative projects. QualCoder doesn't offer a cloud storage service that would enable real-time sharing, but projects can be stored on a secure shared storage platform (such as Google Drive or Microsoft OneDrive) and used by multiple users.

Here are a few tips to keep in mind to improve the collaborative QualCoder experience:

1. Plan ahead to ensure only one collaborator at a time is using the data. Making changes to a project on multiple computers simultaneously may lead to data loss, and you may not even realize anything is missing or corrupted immediately.
2. When working collaboratively, make sure to change the active user in `Project - Settings` every time you open the project. This ensures coding and other changes can be tracked by user, and also allows for later comparison of coding or *inter-rater reliability* calculations with `Coding comparison` reports.
3. If multiple people are coding the same text, it may be easier to agree on a single coding scheme and create the code tree before starting the coding process.
4. If adding codes after initial tree creation in a collaborative project, consider placing them under a `Draft codes` category and using journals or code memos to document your reasoning until you are able to discuss them with your team.

## Exporting project elements

Sometimes, however, you only want to share a specific portion of the project with collaborators. Most views and reports in QualCoder can be exported in a variety of formats, including `XLS` or `CSV` (spreadsheet), `HTML` (webpage), and `TXT` (plain text). Unlike sharing a whole project, exporting individual project elements gives fine-grained control over the setup of the exported file.

## Transparency and reuse

Certain scientific disciplines have called for research transparency, including sharing data and analytic procedures, with momentum growing in many social sciences. Until recently, that effort was primarily applied to quantitative data, such as surveys, experiments, and "big data" gathered from the internet.

A small number of initiatives are working to change that perception and promote the thoughtful, informed, careful sharing of qualitative and mixed methods data as well, led in part by the [Qualitative Data Repository][qdr] and enabled by improvements in sharing like `REFI-QDA`.

## Helping future you

If the arguments above don't convince you that it's good and worth the effort to archive qualitative data securely, there is one more important case to be made.

Archiving your data in an open and interchangeable format that is backed up in multiple locations can help future you. If your only copy of your project is on your laptop and it is lost or destroyed before analysis and review are complete, or if you decide you want to do additional analysis later, there isn't much that can be done short of repeating a large amount of work.

QualCoder only stores data on your computer. Whether or not you plan to share or reuse your data, consider exporting your project at key points, such as after you've completed initial or axial coding.

## Next steps

This lesson has covered basic principles of qualitative research, as well as how to use Taguette for qualitative coding and data analysis. With that foundation, the next step is to find or collect your own data and try it for yourself.

In addition to the Qualitative Data Repository (used and discussed here), some other social science data archives such as ICPSR have qualitative sections. For qualitative content analysis, there are thousands of open-access archives of documents, research, education resources, and even entire books.

:::

::: keypoints

- Archiving and sharing qualitative data can help you, your collaborators, and other researchers
- QualCoder's import and export options can help you share key components of your work
- There are many resources available to continue learning about qualitative research and finding, reusing and sharing qualitative data

:::
