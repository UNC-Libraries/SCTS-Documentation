Updated June 2020


# Overview

- [`<digfolder>` coding in the FAID](#digfolder-coding-in-the-faid)
- [Legacy updates to finding aids](#legacy-updates-to-finding-aid)
- [Statements](#statements)
- [Processing](#processing)
- [MODS requirements](#mods-requirements)
- [CSV to MODS (the Patrick Cullom method)](#cvs-to-mods-the-patrick-cullom-method)
- [Putting Stuff Away](#putting-stuff-away)

***


# `<digfolder>` coding in the FAID

In the example below the key parts of the coding are these two tags:  

```
<container type="digfolder"><extref href=""></extref></container>
```

Href="": Copy the link to the public view of the digital file in the CDR and paste it between the quotation marks.  

**Public view:** https://cdr.lib.unc.edu/list/uuid:f27b77d9-40d0-4e05-9601-5dabcd6372cf 

**Admin view:** https://cdr.lib.unc.edu/admin/list/uuid:f27b77d9-40d0-4e05-9601-5dabcd6372cf 

The admin view can only be accessed by people with admin privileges. 

```
<c02><did><container type="digfolder"> 

<extref href="https://cdr.lib.unc.edu/list/
uuid:f27b77d9-40d0-4e05-9601-5dabcd6372cf">DF-xxxx/x</extref>
</container> 

<unittitle>Reflections of My Life and Ministry</unittitle> 

</did></c02> 
```

Be sure to check that your links are working from the finding aid. 


# Legacy updates to finding aid

1. Update revision description:

   - Insert change tags between revisiondesc tags: 

   ```
   <change> <date>[Month] 2015</date> <item>Finding aid updated for 
   born digital processing by [Name].</item> </change>
   ```

   - Some finding aids might not have revisions description tags. Insert revisiondesc tags between profiledesc and eadheader: ]

   ```
   </profiledesc> <revisiondesc> </revisiondesc> </eadheader>
   ```

2. Update processing info:

   ```
   <processinfo> <head>Processing Information</head> 

   <p>Finding aid updated for born digital processing by [Name], [Month] 
   2015. </p> </processinfo> 
   ```

3. Update items seperated:

   - Remove description of the physical item (FD-, DVD-, DCD-, etc.)  

   - List as Digital Folder (DF-): 

   ```
   <separatedmaterial> <head>Items Separated</head> <list type="simple"> 
   <item>Digital Item (DF-40124/1) available in the    Carolina Digital Repository. 
   </item> </list> </separatedmaterial>
   ```

4. Add an item-level note explainging the files came from legacy media:

   ```
   <c03> <did> <container type="digitem"><extref 
   href="https://cdr.lib.unc.edu/list/uuid:fb046a55-7424-4092-87cf-   
   94af90d054eb">DI-40124/1</extref></container><unittitle>
   North Carolina Fellows Program: <emph render="doublequote">
   Perspectives on Diversity</emph></unittitle> </did> <scopecontent> 
   <p>Produced by the Class of 2005.</p><p>Migrated from DVD-40124/1.
   </p> </scopecontent></c03>
   ```

## In the CDR:

1. Update the MODS:

   - **Title:** Should be the same as the digital item/folder title in the finding aid.

   - **Identifier:** Should be the same as the item/folder number

   - **Example:** DF-40124/1
 
   - **Note:** Add a note explaining the files were migrated from original media

2. Move folders out of unprocessed.

3. Publish items.


# Statements

## Access

### Standard statement for how to get help with file formats that are difficult to access 

Digital files in this collection may contain file formats that users might find difficult to access. For guidance on accessing these files, please email wilsonlibrary@unc.edu.  

### ONYEN access only items

Example: https://finding-aids.lib.unc.edu/40235/#d1e18341

Immediate access to digital files is available for current University of North Carolina at Chapel Hill affiliates with an ONYEN. If you don’t have an ONYEN, contact wilsonlibrary@unc.edu to discuss access options. 

### Metadata only items

Library use only for digital files found in this collection. Contact wilsonlibrary@unc.edu to discuss access options. 

## `<processinfo>`

### At the collection level:

** Regarding processing of back-log born digital:**

```
<p>Finding aid updated for born digital processing by [Name], 
[Month] 2015.</p> 
```

**Regarding obsolete file formats:**

```
<p>Digital files in this collection may contain file formats that users might find difficult to access. For guidance on accessing these 
files, please email wilsonlibrary@unc.edu.</>
```

**Items Separated:**

- List the digital folder number range (DF-70000/1-12).

### At the file level:

**Regarding media that has been retained but not ingested into CDR because it was unreadable with current technology:**

```
<p>Storage media was inaccessible in MONTH YEAR. If you would like to inquire about this item, please email wilsonlibrary@unc.edu</p> 
```

**Regarding media that has been retained per curator but not ingested into CDR:**

```
<p>This file includes media that has been retained for its visual artifactual value.</p> 
```

**Regarding the creation of access files:**

```
<p>An access .mp4 file was made from the DVD files for viewing purposes.</p> 
```

# Processing

UARS Born Digital Lab does all of the processing. Their [workflow documentation](https://sites.google.com/site/wilsonborndigital/home) supports the procedures that UARS follows when ingesting born digital materials and preparing them for Acc2Proc or for TS Archival to describe. The focus is on activities largely outside TS purview, but section 4. Description explains where our work intersects. 

## Storage Media Description

What's this for?

- A description of the type of storage media can be used if it's important to the collection context that the user know the type of storage media a set of digital files was extracted from. This is particularly valuable if we are retaining the media as an object people can view in the reading room.  

- The storage media id, if there is one, is listed in the MODS metadata in the CDR, so it doesn't need to be in the finding aid. Images of the media may also accompany the collection in the CDR, but the images are often not public.  

- This will most often be used for legacy/obsolete storage media and not for other means of digital transfer.  

What's added to the finding aid?  

- Name of the storage media. Can be detailed and include brand information or size capacity or just generic types. For example:  
  - The digital files were extracted from 3.5in Floppy Disks and CDs.  

  - The digital files in this folder were extracted from Iomega 100MB zip disks.  
  
## File Format Description and Preservation Context

What's this for?

- File format information can be retrieved from the repository interface and the PREMIS metadata that is stored with each file, so a detailed listing of file formats is not necessary in the finding aid. However, a brief summary of file formats that will provide the user with valuable information about the collection (software used by a creator or sense of time period of creation) may be appropriate. The important thing is to not spend time listing format information that could easily be generated on demand via metadata in the CDR.  

> Remember that while the current CDR user interface doesn't always present the best file format metadata, the data is there. It's just not always readily apparent on the front end, but is available to staff in FITS extract.  

- If you choose to describe file formats in the collection, describe the original file formats as given to us by the donor.  If derivatives are created for access in the finding aid, create a `<processinfo>` statement at the file level.  

Standard Format Information to be used

- Use file format name.  

- Do not use just an extension. Extensions can be wrong. Not all extensions are well known.  

- The file format name(s) should be taken from FITS extract in the CDR or pre-ingest file format identification record.  

Where does it go?

- Series level note

- Folder/file level note

## Inaccessible Storage Media We're Keeping

What's this for?

- Due to technical limitations we may not be able to access all removable media at the time of acquisition. If it's deemed important to keep the media in case we are able to acquire new technology or fund vendor data recovery, the media should be described in the finding aid.  

- Keeping media that is inaccessible "just in case" should be a rare practice.  

- If we have secured funding for vendor services during initial processing, do not list the item level media. Just wait to add the digital files once the files return from the vendor.  

What is added to the finding aid?

- List media as an item  

- Derive title from label on media, if possible  

- List type of storage media  

- List media id number  

- Note date last attempted to access the media and note that it was inaccessible.  

Suggested wording for this note:

§ Storage media was inaccessible in MONTH YEAR. If you would like to inquire about this item, please email wilsonlibrary@unc.edu.  

Where does it go?

- Item level

- Series level for note about date attempted access if there are many inaccessible disks.

- Include access restriction note

# MODS requirements
 
We have a template built into the CDR. In admin view, you can get to it by clicking on the wheel to the right of a title at any level of a CDR collection:  

1. Click on "Edit Description" in the drop-down menu. 

2. Select "Archival Folder." 

In the template, you should always fill in:

1. The mods title (folder title)

2. The identifiers (accession number and digital folder number)

3. Related item (the URL for the finding aid)

There is a field for another related item, the original storage media, but it is not required and only entered by curatorial request. 

**Anything from the MODS template that isn’t needed should be removed. For example, if we are not recording the source media in the MODS record, we should delete that part of the template.**

# CVS to MODS (the Patrick Cullom method)

THIS MAY NEED UPDATE AS OF 1/2/2018

This is an especially useful workflow if you are processing more than a handful of digital folders. You can export the folder titles, edit them as needed, and create the mods records for each folder all in one excel spreadsheet that you will re-upload back into the CDR. 

[CDR CSV to Mods](https://adminliveunc.sharepoint.com/:p:/r/sites/lib/departments/wts/_layouts/15/WopiFrame.aspx?sourcedoc=%7B675ECBEB-1D39-428E-94A1-E2CF3D143A55%7D&file=CDR_CSV_to_MODS_REVISED.pptx&action=default)

# Putting stuff away

There are currently three locations to shelve physical born-digital materials:

**1. Materials ingested into the DCR**: Level 6, Black, , Y Range 9, Side b.

   Ingested materials are stored in shared boxes, "Digital Storage Device Box", on Level 6. Harddrives and other larger items may be shelved as-is on the shelf.
   
   Record the location of these materials in the appropriate accession record in ArchivesSpace as an Instance. Under instance, browse or create the appropriate shared Digital Storage Device Box. No need to list individual items, just a box location will do. If you have a larger item that is not in a shared box, list the location in the "General Note" field of the accession record.

**2. Materials awaiting ingest or further appraisal**; Level 6, Black, Black, Y Range 10, Side a.

   Materials awaiting ingest are shelved as-in by accession on Level 6.
   
   Record the location of these in the appropriate accession record in ArchivesSpace in the General Note field.

**3. Legacy materials already listed in finding aids** (FLD-, CD-, DVD-, etc): Level 6, Black, T Range 2, Side b.

   Legacy materials are shelved in various shared boxes on Level 6.
   
   Locations for these materials are listed in the appropriate Resource record. Please note that many of the materials are not listed in the collection finding aid they belong to. 


