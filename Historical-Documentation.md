Updated August 2025


# Overview

- [Style](#style)
   - [Military Papers](#military-papers)
   - [Literary Papers](#literary-papers)
- [Mechanics](#mechanics)
     - [XML to TXT script](#xml-to-txt-script)
   - [Excel formulas/tips](#excel-formulastips) 
- [EAD Documentation](#ead-documentation)
   - [Additions](#additions)
- [Identity Statement](#identity-statement)
   


***
# Style

How we process archival collections has evolved over time. Since implementation of a local version of More Product, Less Process (MPLP), we have significantly curtailed the depth to which we describe collection materials. Included here is descriptive guidance that is not wrong, but it is generally not in active use because we are not doing in-depth processing. 




## Military Papers

When describing an oral history of or a letter written by a soldier, if possible, include the following in the biographical and scope and content notes:

- the regiment in which the writer served

- if the writer was a soldier or an officer

- where the writer was writing from and where he was writing to (if this is a quick processing job, you can often tell by looking at the very top of the letter and seeing where the writer was positioned—which makes you able to say, for example, that he was writing from Virginia, without reading more in depth)

- what places are referenced in the letters or oral history

- what battles are being described

If you are describing the letters in more depth, you can include information about camp life, sickness, death, and other cheerful wartime subjects.  

## Literary papers

**Life Cycle of a Publication**

![idea to book figure](https://user-images.githubusercontent.com/58087302/80127592-8a315700-8562-11ea-98ab-fdd2623d2a27.jpeg)


# Mechanics

## XML to TXT script

Use the Saxon script to convert finding aid XML files to TXT files. This is an easy way to get finding aid data into a spreadsheet friendly format. Please note this script only exports limited fields from the XML file. At this time, nothing below the item title (i.e. `<genreform>`, `<scopecontent>`) can be exported through this script). The Saxon script exports the following fields from the XML file: 

- Collection Name 
- Collection Number 
- Location in Collection 
- Object (contains hook_id and item title) 
- Preferred Citation 
- Container Type 
- hook_id 
- Usage rights

### Instructions

**1.** Copy the “saxon” folder from the Tech Services Louis page to your desktop (Departmental Documents>TS_Archival>saxon): https://adminliveunc.sharepoint.com/:f:/r/sites/lib/departments/wts/Shared%20Documents/TS_Archival/saxon?csf=1&e=3hE3Ul 

**2.** Make a copy of the xml file for the finding aid. Put the copy in the saxon folder on your desktop. 

**3.** Open command line and type in the following commands 

   ```
   cd desktop/saxon;  

   java -jar saxon9he.jar -o :[insert name of output text file] 
   [insert name of finding aid file] ead2cdm_automate.xsl 
   ```
   
**Example command for 20367 finding aid:**

   ```
   Example command for 20367 finding aid:  

   java -jar saxon9he.jar -o:20367.txt 20367.xml ead2cdm_automate.xsl 
   ```

**4.** The txt file for your XML file should now be in the Saxon folder on your desktop. Open Excel and then open the txt file you just created (note "All files" must be selected in order to see your new txt file). Select "Next", "Next", "Finish" on the 3 window Text Import Wizard prompt. 

Voila!

You can manipulate these fields to fit your needs. For example, use find and replace to change "hook_id" into item call numbers (ex: folder_1 to F-20367/1).  


## Excel formulas/tips

### Deleting empty cells

Home tab-->Find & Select-->Go to Special...-->Blanks 

Home tab-->Delete-->Delete cells 

### Breaking apart strings of text

Delimit by characters (will delimit by every instance of this character within the string) 

   Data tab-->Text to Columns-->Delimit-->Choose your delimiters 
   
By Formula (can delimit by only first instance of character) 

```
=LEFT(A1,FIND("[delimiter]",A1)-1)  

=RIGHT(A1,LEN(B1)-FIND("[delimiter]",A1)) 
```
 
**Example:**

T-40328/1 Mix 1  in column A 

To break apart by first space so you can have "T-40328/1" in one column and "Mix 1" in another, use  

```=LEFT(A1,FIND(" ",A1)-1) and =RIGHT(A1,LEN(B1)-FIND(" ",A1))``` 

# EAD Documentation 

## Additions

**Revising the XML**

This section deals with revisions to finding aids that have already been encoded in EAD. Some may have originally been SGML documents from back in the old days of EAD. These SGML documents have now been converted to XML. Documents that started out in XML will have commented-out revision tags that you can activate. Finding aids converted from SGML won't have those commented-out tags.

The `<revisiondesc>` tag in the `<eadheader>` is where EAD keeps track of revisions. However, the information coded in the `<eadheader>` section doesn't show up on the screen. Therefore, to track revision information and to make the same information visible on the screen, you must enter the information in both the `<revisiondesc>` tags in the `<eadheader>` and the `<processinfo>` section in `<archdesc>`. In both places, how you enter the information is determined by whether or not you're the first one in with a revision.

**Adding revision statements to `<revisiondesc>` in the `<eadheader>`:**

If you're revising an EAD-encoded finding aid that was written in the 2000s and later, the `<revisiondesc>` tags for entering revision information in the `<eadheader>` should be the first commented-out area you encounter:

```
<!--OPTIONAL TAG: use only if revising EAD-encoded finding aid. 
<revisiondesc><change><date>Date of change</date><item>
Updated because of ?</item></change></revisiondesc>-->
```

If you're making the first revision to an EAD-encoded finding aid that was written in the 1990s-early 2000s, you may have to add the `<revisiondesc>` tags after `</profiledesc>` and before `</eadheader>`:

```
</profiledesc><revisiondesc><change><date>May 2020</date>
<item>Updated because of addition (Acc. 20200224.1) 
by Nancy Kaiser</item></change></revisiondesc> </eadheader>
```

If yours is NOT the finding aid's first revision (there's already a `<revisiondesc>` section, just add a new set of <change> tags:

```
<change><date>February 2020</date><item>Updated for addition 
(Acc. 20200110.4) by Nancy Kaiser</item></change>
```

**Adding revision statements to `<processinfo>` in `<archdesc>`:**

We are committed to transparency so you'll also need to add revision information to <archdesc> so that it will display in the finding aid. For minor additions, you may just be adding another name and date to the processing information already there.

```
<processinfo><head>Processing Information</head>
<p>Processed by: Nancy Kaiser, January 2010</p>
<p>Encoded by: Nancy Kaiser, January 2010</p>
<p>Revisions by: Anne Wells, April 2017; 
Patrick Cullom, January 2020; (your name, date).</p>
</processinfo>
```

When multiple people are involved in preparing a collection for discovery and use, it will be appropriate to use our more inclusive processing info statements <link> that acknowledge the expertise brought to bear by our collecting and format specialist colleagues. 

**Other parts of the finding aid that may or may not require updates:**

[Title and Date](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#title-and-date): Sometimes you will change a title from something narrow like Roslyn P. Holdzkom Diaries, to Roslyn P. Holdzkom Papers because the addition included other formats besides diaries.

> Note: Don’t miss any of the 3 collection level places and the series level when editing date information.
```
<titlestmt> <titleproper encodinganalog="title">

<frontmatter> <titlepage> <titleproper>

<unittitle label="Title" encodinganalog="245">
```
  
[Extent](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#extent): This will almost certainly change. 

[Abstract and Collection Overview](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#scope-and-content-note-and-abstract): You may or may not need to edit this. If nothing else, 1) check to see if 545 tag is in use. If so, move content from the 545 to the 520 tags and then delete the 545; and 2) check to be sure racial and ethnic identity have been updated. If you are adding identity information, be sure to add the identity statement <link> to the <processinfo>.
  
Collection overview: This will change, even if the abstract does not. Typically you will add a sentence or two that begins with “The Addition of May 2020 consists of ….” You can use the same description in the series description.

[Acquisition](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#acquisition): Information should be updated to include the donor, date, and accession information.

If you have a separately maintained addition that has been appended to the end with little description, it’s good practice to warn researchers in the collection overview that they will need to look in the collection's additions to find all the materials of interest. 
Example: Additions received after 1979 have not been integrated into the original deposit. Researchers should always check additions to be sure they have identified all files of interest to them.

[Restriction](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#restrictions): Add or remove restrictions as needed. Be sure to add or remove the restriction at every level: collection, series, and container.

**Between the `<dsc>`:**

When you add your new series, whether integrated intellectually or appended to the end, it should look like this:

*Title, inclusive dates, (Addition of ____).*
```
<c01 level="series"><did><unittitle>Papers and Digital Files, <unitdate 
normal="1990/2000" type="inclusive">1990-2000</unitdate> (Addition of January 2020).
</unittitle>
```
*Extent: linear feet and/or items / gigabytes and/or digital files*
```
<physdesc><extent>1.0 linear feet (1000 paper items) / 1 gigabyte (17 digital files).</extent>
</physdesc><did>
```
**Arrangement: if archivist imposed any arrangement, put that information in a processing note**

Most likely you are just rehousing into 
archival boxes
```
<arrangement><p>Arrangement: as received.</p></arrangement>
```
**Acquisitions**

Include all accession numbers at the series level.
```
<acqinfo><p>Acquisitions Information: Accession 20200124.2</p></acqinfo>
```
**Processing Note**

Sometimes we want to communicate to researchers 
that we really do not know what is in the addition we are making available for use. 
Be sure to use one of the boilerplate notes for [first pass processing](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#processing-information). This is also where 
you will note any archivist interventions, such as arrangement imposed or materials 
appraised out of the addition.
```
<processinfo><p>Processing Note: </p></processinfo>
```
**Scope and Content**

Probably this will be same brief description
as you added to the Collection Overview
Probably this will be same brief description
as you added to the Collection Overview
```
<scopecontent><p>Overview of the addition.</p></scopecontent>
```
**Container list**
```
<c02><did><container type=”box”>19</container><unittitle>Papers, 1990-2000</unittitle>
</did></c02></c01>

<c02><did><container type=”digfolder”><extref href=”lettersandnumbers”>DF-90999/1</extref>
</container><unittitle>Papers, 1990-2000</unittitle></did></c02>
</c01>
```

# Other Unusual Situations

## Drop-ins

Occasionally it makes sense to drop a single item or two in with the original deposit. This does not mean that we have stopped caring about provenance! Enclose your item in a piece of archival paper and write the accession number on the outside before dropping into an existing folder.

In the finding aid:

You still have to record the edits in the <revision> section, and to update the acquisitions information at the collection level. Because we do drop-ins only for items with low anticipated research value, it is less likely that you will need to amend title, collection dates, extent, and abstract. Of course you should make those changes as needed.

Also add an `<acqinfo>` statement at the container level:

```
<c02><did><container type=”folder”>100</container><unittitle>
Correspondence, 1865</unittitle></did><acqinfo><p>Acquisitions Information: 
Letter, 10 April 1865, was received as Accession 109832</p></acqinfo></c02>
```

> Note: drop-ins are not an option for collections/containers that have been microfilmed or digitized.

## Folder only

Similarly, it occasionally makes sense to integrate a single folder into the original deposit rather than to create a new series. Unlike drop-ins, this addition likely will be filed physically at the end of the collection but will be listed with the original deposit where it fits intellectually. 

Write "Addition of ___" and the accession number on the folder.

In the finding aid, add an `<acqinfo>` statement at the container level:

```
<c02><did><container type=”audiotape”>F-20025/934</container><unittitle>
Bluegrass performance, 1978</unittitle></did><acqinfo><p>Acquisitions Information: 
Accession 109832</p></acqinfo></c02>
```

And at the series level:

```
<acqinfo><p>Acquisitions Information: F-20025/934 received as Addition 
of October 2016 (Acc. 102664).</p></acqinfo>
```

Sometimes not all the materials in the addition will be made usable at the same time, especially when there are born digital materials. Be sure to add one of the Access Restriction statements if that is the case. 

# Identity Statement

Older version of the statement to acknowledge ethnic and racial identities for individuals and families represented in collections (discontinued in July 2025):

Since August 2017, we have added ethnic and racial identities for individuals and families represented in collections. To determine identity, we rely on self-identification; other information supplied to the repository by collection creators or sources; public records, press accounts, and secondary sources; and contextual information in the collection materials. Omissions of ethnic and racial identities in finding aids created or updated after August 2017 are an indication of insufficient information to make an educated guess or an individual's preference for identity information to be excluded from description. When we have misidentified, please let us know at wilsonlibrary@unc.edu.

