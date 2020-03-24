# Overview

- Introduction
- Drop-ins (items)
- Integrated Additions (series)
- 2 Integrated Additions (folder)
- Seperately Maintained Additions
- Unprocessed Additions: Statement
- Revisions to XML
- Processing Note: Statements
- ```<acqinfo>```

***

# Introduction

We often receive material that is related to collections that are already here. Instead of making a new collection, we add this material to the existing collection, hence the name Addition. When faced with an addition, the first decision that must be made is whether to incorporate the addition into the arrangement of the original deposit or to add the additional materials at the end of the original deposit’s arrangement in what we call a separately maintained addition.  

In some cases, it may be very easy to drop materials into the appropriate places in the original deposit without changing the arrangement or description. However, before integrating materials consider how the collection has already been used. Some collections are heavily used by repeat researchers who may find confusing the intermingling of new material with old. Also, for some collections, it might make sense to highlight new material, even if it is just one letter. It is a good idea to consult with your supervising archivist for help with the decision to interfile or to create a separate addition. If you do interfile, be sure to put a note in the control file indicating what, where, and when new material was interfiled.  

More frequently, you will opt for creating separately maintained additions; these can come in many styles. If the materials in the addition mimic the materials in the original deposit you can use the same arrangement in your addition. The materials do not have to correspond exactly. For example, in your original deposit, you might have Series 1. Correspondence, Series 2. Diaries, and Series 3. Pictures. It is fine for your addition to have a diaries series; a pictures series; and a new series of audio-visual materials. Of course, materials in the addition may not have anything to do with the original deposit. In that case, it is completely fine to devise a new arrangement for them. 

See the pages for Drop-ins, Integrated Additions, and Separately Maintained Additions in this section. 


# Drop-ins (items)

Occasionally it makes sense to drop a single item or two in with the original deposit. This does not mean that we have stopped caring about provenance! Enclose your item in a piece of archival paper and write the accession number on outside before dropping into an existing folder. In the finding aid, add an < acqinfo > statement at the container level: 

```<acqinfo><p>Acquisitions Information: Letter, 10 April 1865, was received as Accession 109832</p></acqinfo>```

> Note: drop-ins are not an option for collections/containers that have been microfilmed or digitized. 


# Integrated Additions (series)

In some cases you will decide it is both efficient and more transparent to do some top level intellectual arrangement.  This may be the case when you have a large collection with an extensive contents list in which the addition is likely to be lost at the end for most researchers.  

You will add an "A" to the series number to indicate that it is an addition and include a parenthetical at the end to identify which addition (as collections can have many additions). You will also add ```<acqinfo>``` tags to indicate the accession number. In this example, there have been two additions to the correspondence series, one in March 2008 and one in April 2010. 

When you have material that falls outside the existing series, add a new one, with the "A" to indicate that it was part of an addition. In this example, a photographs series is new with the Addition of March 2008. 

> Note that these additions are not physically integrated with the original deposit. 

#### Series 1. Correspondence and related materials

Folder 1 Correspondence, 1901-1910 

Folder 2 Correspondence, 1911-1920 

Folder 3 Correspondence, 1921-1945 

#### Series 1A. Correspondence (Addition of March 2008)  

```<acqinfo><p>Acquisitions Information: Accession 10452</p></acqinfo>```

**_Folder 6 Correspondence, 1927_**

**_Folder 7 Correspondence, 1956_**

#### Series 1A. Correspondence (Addition of April 2010)

```<acqinfo><p>Acquisitions Information: Accession 19874</p></acqinfo>```

**_Folder 8 Correspondence, 1920-1930 _**

#### Series 2.Diaries  

Folder 4 Diary, 1925 

Folder 5 Diary, 1942  

#### Series 3A. Photographs (Addition of March 2008)  

```<acqinfo><p>Acquisitions Information: Accession 10452</p></acqinfo>```

**_Image folder PF-09999/1 Photographs, 1927_**


# 2 Integrated Additions (folder)

Occasionally it makes sense to integrate a folder into the original deposit rather than to create a new series. Unlike drop-ins, this addition likely will be filed physically at the end of the collection but will be listed with the original deposit where it fits intellectually.  This does not mean that we have stopped caring about provenance! Write "Addition of ___" and the accession number on the folder.  

In the finding aid, add an < acqinfo > statement at the container level: 

```<acqinfo><p>Acquisitions Information:  Accession 109832</p></acqinfo>```

And at the series level: 

```<acqinfo><p>Acquisitions Information:  F-20025/934 received as Addition of October 2016 (Acc. 102664).</p></acqinfo>```

# Seperately Maintained Additions

## Additions at the End

The quickest way to handle additions is usually to add them on to the end of the finding aid with no arrangement or intellectual integration of the material.  In the first example, there are three additions, one in March 2008, one in January 2012, and one in February 2017. Sometimes there is material that overlaps with the original deposit and sometimes there is new material that does not.  The second example is a full-blown finding aid in which all of the changes are bolded. 

If the contents list begins to get unwieldy and hard to penetrate, think about going the route of integrated additions. 

## Example 1

### Contents List

#### Series 1. Correspondence and related materials

Folder 1 Correspondence, 1901-1910 

Folder 2 Correspondence, 1911-1920 

Folder 3 Correspondence, 1921-1945 

#### Series 2. Diaries

Folder 4 Diary, 1925 

Folder 5 Diary, 1942  

#### Series 3. Additions

#### 3.1. Correspondence and Photographs (Addition of March 2008)

```<acqinfo><p>Acquisitions Information: Accession 10452</p></acqinfo>```

**_Folder 6 Correspondence, 1946_**

**_PF-09999/1 Photographs, 1900s-1920s_** 

#### 3.2. Account Books (Addition of January 2012)  

```<acqinfo><p>Acquisitions Information: Accession 19567</p></acqinfo>```

**_Folder 7 Account book, 1901_**

**_Folder 8 Account book, 1902-1903_**

#### Account Book and Photographs (Addition of February 2017)  

```<acqinfo><p>Acquisitions Information: Accession 200135</p></acqinfo>```

**_Folder 9 Account book, 1905_**

**_PF-09999/2 Photographs of Hetty Holdzkom, 1903_**

## Alerting Researchers to Additions

With separately maintained additions, it's good practice to warn researchers that they will need to look in the collection's additions to find all the materials that they need. Include a note indicating this as the last paragraph of your scope and content note.  

_Example of a collection level scope content note alerting researchers about additions:_

These papers consist chiefly of family letters from the 1790s through the early 1860s. Correspondence of the family with outsiders had been almost entirely excluded from the collection, but family letters were deliberately preserved as a "family record" (see Ellen Mordecai's letters of October-November 1854). The Addition of January 2007 includes personal letters between family members; 1816 letters by Maria Edgeworth and Richard Lovell Edgeworth responding to Rachel Mordecai Lazarus's letter concerning Edgeworth's literary treatment of Jews; and reminiscences, song lyrics, and fragments. The Addition of September 2007 includes letters written to and by Mordecai family members, 1865 and 1916-1917, and one poem dated 1945. The Addition of December 2007 contains the three-volume "A Memoir of Maria Edgeworth with a Selection from Her Letters by the late Mrs. Edgeworth" (unpublished) with accompanying notes tipped in.  

Additions received after 1979 have not been integrated into the original deposits. Researchers should always check additions to be sure they have identified all files of interest to them. 


# Unprocessed Additions: Statement

The following statement should go in the **Access Restrictions** element for collections having unprocessed additions: 

_This collection contains additional materials that are not processed and are currently not available to researchers. For information about access to these materials, contact Research and Instructional Services staff. Please be advised that preparing unprocessed materials for access can be a lengthy process._

When an addition is described in the finding aid to make the content discoverable, but it has not been made usable: 

_This addition is not available for immediate or same day access. Please contact Research and Instructional Service staff at wilsonlibrary@unc.edu to discuss options for consulting this collection._


# Revisions to XML

This section deals with revisions to finding aids that have already been encoded in EAD. Some may have originally been SGML documents from back in the old days of EAD. These SGML documents have now been converted to XML. Documents that started out in XML will have commented-out revision tags that you can activate. Finding aids converted from SGML won't have those commented-out tags.  

The ```<revisiondesc>``` tag in the ```<eadheader>``` is where EAD keeps track of revisions. However, the information coded in the < eadheader > section doesn't show up on the screen. Therefore, to track revision information and to make said information visible on the screen, you must enter the information in both the ```<revisiondesc>``` tags in the ```<eadheader>``` and the ```<processinfo>``` section in ```<archdesc>```.  

In both places, how you enter the information is determined by whether or not you're the first one in with a revision.  

## Adding revision statements to ```<revisiondesc>``` in the ```<eadheader>```: 

If you're revising an EAD-encoded finding aid that was written fairly recently, the ```<revisiondesc>``` tags for entering revision information in the ```<eadheader>``` should be the first commented-out area you encounter:  

```<!--OPTIONAL TAG: use only if revising EAD-encoded finding aid.<revisiondesc><change><date>Date 
of change</date><item>Updated because of ?</item></change></revisiondesc>-->```

If you're making the first revision to an EAD-encoded finding aid that was written when we first starting doing EAD, you may have to add the ```<revisiondesc>``` tags. Place your cursor after ```</profiledesc>``` and before ```</eadheader>``` and add

```
</profiledesc>  

<revisiondesc><change><date>(add month and year of revision)</date> 

<item>Updated because of (say why you're updating--addition/donor request/corrections, etc.) by 
(your name)</item> 

</change></revisiondesc> 

 </eadheader> 
 ```
 
 If yours is NOT the finding aid's first revision (there's already a ```<revisiondesc>``` section, just add a new set of ```<change>``` tags:  

```<change><date></date><item></item></change>```  

## Adding revision statements to ```<processinfo>``` in ```<archdesc>```:

You'll also need to add revision information to ```<archdesc>``` so that it will display. You needn't give a reason for revising here. You may have to turn the ```<processinfo>``` tags on or you may just be adding another to processing information already there. If the latter, you can use this template:  

```<p>Revisions: Finding aid updated in <date>(add month and year of revision)</date> by (your name).</p>```

Here's a full-blown example of a modern ```<processinfo>``` with a revision statement:  


```<processinfo><head>Processing Information</head><p>Processed by: Carolyn Wallace, 1969; William Auman,
1985; Roslyn Holdzkom, 1996</p>

<p>Encoded by: Roslyn Holdzkom, November 2003</p> 

<p>This collection was processed with support from the National Endowment for the Humanities.</p><p>The Addition
of November 2001 is arranged in the same way as, but has not been incorporated into, the original deposit of 
materials.</p>

<p>Additions received after February 1995 have not been integrated into the original deposits. Researchers should 
always check additions to be sure they have identified all files of interest to them.</p> 

<p>Finding aid updated in January 2004 by Roslyn Holdzkom because of addition.</p> 

</processinfo>```


Revisions can be made ad nauseam. Just keep piling them on, but feel free to do some logical consolidation of entries if things seem to be getting out of hand.  

## Adding Missing Tags

If you're revising a pre-XML EAD-encoded finding aid, you may find that some tags are missing. Three of the most common missing tags that you might want to add are available in the Other Elements section of the clip sidebar.  

### ```<prefercite>``` 

It's always a good idea to add ```<prefercite>``` if there isn't one. Add ```<prefercite>``` after ```<processinfo>```. If there's no ```<processinfo>```, add ```<prefercite>``` after ```<acqinfo>```. You'll have to fill in the collection name, collection number, and edit the repository name.  

```
<prefercite encodinganalog="524"><head>Preferred Citation</head><p>[Identification of item], in the [name of collection] #[collection number], [chose one: Southern Historical Collection, Southern Folklife Collection, University Archives, General Manuscripts], Wilson Library, University of North Carolina at Chapel Hill.</p></prefercite>
```

### ```<processinfo>``` 

If you need to add a ```<processinfo>```, do so after ```<acqinfo>```.  

```
<processinfo><p>Processing Note: Enter Note.</p></processinfo>
```

### ```<accessrestrict>``` and ```<userestrict>``` 

You may need to add ```<accessrestrict>``` and ```<userestrict>```. ```<userestrict>``` must follow ```<accessrestrict>```. If there's no ```<accessrestrict>```, add one. Add ```<accessrestrict>``` right after ```<head>Administrative Information</head>``` and ```<userestrict>``` right after ```<accessrestrict>```.  

```
<accessrestrict encodinganalog="506"><p>Restriction: Enter Restrictions Note.</p></accessrestrict><userestrict><p>Use Restriction: Enter Restrictions Note.</p></userestrict> 

<p>Additions received after February 1995 have not been integrated into the original deposits. Researchers should always check additions to be sure they have identified all files of interest to them.</p> 

<p>Finding aid updated in January 2004 by Roslyn Holdzkom because of addition.</p></processinfo>  
```


# Processing Note: Statements

The Addition of November 2001 is arranged in the same way as, but has not been incorporated into, the original deposit of materials. 

Additions received after February 1995 have not been integrated into the original deposit. Researchers should always check additions to be sure they have identified all files of interest to them. 

The Addition has been intellectually integrated with the original deposit but is distinguishable by accession information.   


# ```<acqinfo>```

We have always used ```<acqinfo>``` to record the collection provenance in the front part of the finding aid. Since 2016 we have taken to using it more liberally throughout a finding aid to record new accessions to the same collection.  

Use ```<acqinfo><p></p ></acqinfo>``` at the container level when you are intellectually integrating an addition into a finding aid (even though physically it will live elsewhere).  

At the container level, include a label and either an addition statement or accession number or both: 

```<acqinfo><p>Acquisition information: Addition of April 2004 (Acc. 101003)</p></acqinfo>``` 

You can also use it for an additions series. If you have an additions series, an addition statement will be part of the title. Use ```<acqinfo>``` for the accession number:

```
<c02><did><unittitle>Correspondence, 1990-1992: Addition of June 1994</unittitle></did> 

<acqinfo><p>Acquisition Information: Acc. 101003<p></acqinfo> 

</c02> 
```
