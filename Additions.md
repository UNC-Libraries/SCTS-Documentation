# Overview

- [Arrangement](#arrangement)
- [Revising the XML](#revising-the-xml)
- [Other Unusual Situations](#other-unusual-situations)

***

# Arrangement

We often receive material that is related to collections that are already here. Instead of making a new collection, we add this material to the existing collection. Additions are maintained separately in a physical sense, but we try to integrate them intellectually with materials received previously to facilitate discovery. Sometimes this is easily done; sometimes it is better to append new description to the end of the finding aid.

If the materials in the addition clearly mimic the materials in the original deposit you can use the same arrangement in your addition. 

> Note that the “A” is for Addition, to distinguish it from the original deposit. Use the “A” whether you are adding to an existing series or creating a new one. Always add the date of the accession in parentheses after the series title.

Series 1. Correspondence

**Series 1A. Correspondence (Addition of January 2000)**

Series 2. Diaries

Series 3. Pictures



Perhaps the addition consists of several different kinds of materials. For a variety of reasons, it may not make sense to divide these up according to the original series arrangement:

Series 1. Correspondence

Series 2. Diaries

Series 3. Pictures

**Series 4A. Papers (Addition of February 2005)**


Many of our collections receive subsequent additions over many years. You may use multiple different strategies.

Series 1. Correspondence

**Series 1A. Correspondence (Addition of April 2000)**

Series 2. Diaries

Series 3. Pictures

**Series 4A. Papers (Addition of February 2005)**

**Series 4A. Papers (Addition of April 2015)**

**Series 5A. Audio Visual (Addition of March 2010)**

**Series 5A. Audio Visual (Addition of April 2015)**


Sometimes with organizational records and family collections with a lot of additions, it is easiest just to append the additions to the end, with no arrangement or intellectual integration of the material. Sometimes there is material that overlaps with the original deposit and sometimes there is new material that does not. Until researcher interest proves otherwise, we simply note
the additions and move on.

1. Foundation Records, 1990-1995 (Original Deposit).

**2A. Foundation Records, 1986-1988 (Addition of May 1996).**

**2A. Foundation Records, 1983-1989 (Addition of March 1997).**

**2A. Foundation Records, 1970-1992 (Addition of March 1998).**


We have a long and complicated history with additions so you might encounter all kinds of variations on the above examples. Usually it is most expedient to follow the arrangement that already exists, though sometimes it makes sense to do minor re-coding to bring clarity. 


# Revising the XML

This section deals with revisions to finding aids that have already been encoded in EAD. Some may have originally been SGML documents from back in the old days of EAD. These SGML documents have now been converted to XML. Documents that started out in XML will have commented-out revision tags that you can activate. Finding aids converted from SGML won't have those commented-out tags.

The `<revisiondesc>` tag in the `<eadheader>` is where EAD keeps track of revisions. However, the information coded in the `<eadheader>` section doesn't show up on the screen. Therefore, to track revision information and to make the same information visible on the screen, you must enter the information in both the `<revisiondesc>` tags in the `<eadheader>` and the `<processinfo>` section in `<archdesc>`. In both places, how you enter the information is determined by whether or not you're the first one in with a revision.

_Adding revision statements to `<revisiondesc>` in the `<eadheader>`:_

If you're revising an EAD-encoded finding aid that was written in the 2000s and later, the `<revisiondesc>` tags for entering revision information in the `<eadheader>` should be the first commented-out area you encounter:

`<!--OPTIONAL TAG: use only if revising EAD-encoded finding aid. <revisiondesc><change><date>Date of change</date><item>Updated because of ?</item></change></revisiondesc>-->`


If you're making the first revision to an EAD-encoded finding aid that was written in the 1990s-early 2000s, you may have to add the `<revisiondesc>` tags after `</profiledesc>` and before `</eadheader>`:

```
</profiledesc><revisiondesc><change><date>May 2020</date><item>Updated because of addition (Acc. 20200224.1) by Nancy Kaiser</item></change></revisiondesc> </eadheader>
```

If yours is NOT the finding aid's first revision (there's already a `<revisiondesc>` section, just add a new set of <change> tags:


`<change><date>February 2020</date><item>Updated for addition (Acc. 20200110.4) by Nancy Kaiser</item></change>`


_Adding revision statements to <processinfo> in <archdesc>:_

We are committed to transparency so you'll also need to add revision information to <archdesc> so that it will display in the finding aid. For minor additions, you may just be adding another name and date to the processing information already there.


`<processinfo><head>Processing Information</head>
<p>Processed by: Nancy Kaiser, January 2010</p>
<p>Encoded by: Nancy Kaiser, January 2010</p>
<p>Revisions by: Anne Wells, April 2017; Patrick Cullom, January 2020; (your name, date).</p>
</processinfo>`


When multiple people are involved in preparing a collection for discovery and use, it will be appropriate to use our more inclusive processing info statements <link> that acknowledge the expertise brought to bear by our collecting and format specialist colleagues. 

Other parts of the finding aid may or may not require updates.

[Title and Date](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#title-and-date): Sometimes you will change a title from something narrow like Roslyn P. Holdzkom Diaries, to Roslyn P. Holdzkom Papers because the addition included other formats besides diaries.

Don’t miss any of the 3 collection level places to edit date information.

[Extent](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#extent): This will almost certainly change. 

[Abstract and Collection Overview](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#scope-and-content-note-and-abstract): You may or may not need to edit this. If nothing else, check to be sure racial and ethnic identity have been updated. If you are adding identity information, be sure to add the identity statement <link> to the <processinfo>.
  
Collection overview: This will change, even if the abstract does not. Typically you will add a sentence or two that begins with “The Addition of May 2020 consists of ….” You can use the same description in the series description.

[Acquisition](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#acquisition): Information should be updated to include the donor, date, and accession information.


If you have a separately maintained addition that has been appended to the end with little description, it’s good practice to warn researchers in the collection overview that they will need to look in the collection's additions to find all the materials of interest. 
Example: Additions received after 1979 have not been integrated into the original deposit. Researchers should always check additions to be sure they have identified all files of interest to them.


_Between the `<dsc>`:_ 

When you add your new series, whether integrated intellectually, or appended to the end, it should look like this:


`<c01 level="series"><did><unittitle>Papers and Digital Files, <unitdate normal="1990/2000" type="inclusive">1990-2000</unitdate> (Addition of January 2020).</unittitle>`


`<physdesc><extent>1000 paper items / 1 gigabyte (17 digital files).</extent></physdesc><did>`


`<arrangement><p>Arrangement: as received. (Most likely you are just rehousing into archival boxes.)</p></arrangement>`


`<acqinfo><p>Acquisitions Information: Accession 20200124.2)</p></acqinfo>`


`<processinfo><p>Processing Note: Sometimes we want to communicate to researchers that we really do not know what is in the addition we are making available for use. Be sure to use one of the boilerplate processing notes <link>. This is also where you will note any archivist interventions, such as arrangement imposed or materials appraised out of the addition.</p></processinfo>`


`<scopecontent><p>Overview of the addition. (Probably this will be same brief description as you added to the Collection Overview.</p></scopecontent>`


`<c02><did><container type=”box”>19</container><unittitle>Papers, 1990-2000</unittitle></did></c02></c01>`

`<c02><did><container type=”digfolder”><extref href=”lettersandnumbers”>DF-90999/1</extref></container><unittitle>Papers, 1990-2000</unittitle></did></c02>
</c01>`


# Other Unusual Situations

_Drop-ins_

Occasionally it makes sense to drop a single item or two in with the original deposit. This does not mean that we have stopped caring about provenance! Enclose your item in a piece of archival paper and write the accession number on the outside before dropping into an existing folder.

In the finding aid:

You still have to record the edits in the <revision> section, and to update the acquisitions information at the collection level. Because we do drop-ins only for items with low anticipated research value, it is less likely that you will need to amend title, collection dates, extent, and abstract. Of course you should make those changes as needed.

Also add an < acqinfo > statement at the container level:

`<c02><did><container type=”folder”>100</container><unittitle>Correspondence, 1865</unittitle></did>
<acqinfo><p>Acquisitions Information: Letter, 10 April 1865, was received as Accession 109832</p></acqinfo></c02>`

>Note: drop-ins are not an option for collections/containers that have been microfilmed or digitized.


_Folder only_

Similarly, it occasionally makes sense to integrate a single folder into the original deposit rather than to create a new series. Unlike drop-ins, this addition likely will be filed physically at the end of the collection but will be listed with the original deposit where it fits intellectually. 

Write "Addition of ___" and the accession number on the folder.

In the finding aid, add an <acqinfo> statement at the container level:

`<c02><did><container type=”audiotape”>F-20025/934</container><unittitle>Bluegrass performance, 1978</unittitle></did>
<acqinfo><p>Acquisitions Information: Accession 109832</p></acqinfo></c02>`


And at the series level:


`<acqinfo><p>Acquisitions Information: F-20025/934 received as Addition of October 2016 (Acc. 102664).</p></acqinfo>`


Sometimes not all the materials in the addition will be made usable at the same time, especially when there are born digital materials. Be sure to add one of the Access Restriction statements if that is the case. 
