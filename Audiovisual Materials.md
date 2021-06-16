Content owner: **Anne Wells**

Updated June 2021 by Anne Wells.

# Overview
- [Introduction](#introduction)
- [Arrangement](#arrangement)
- [Jitterbug](#jitterbug)  
    -[Metadata](#metadata)  (call numbers, required & suggested fields, field definitions & style guide, creating titles)  
    -[Data entry and import](#data-entry-and-import)  
    -[Data export](#data-export) 
- [Finding aid description](#finding-aid-description)  
    -[Formats/container types](#formatscontainer-types)  
    -[XML/EAD](#xmlead)  
    -[LC Subject Headings](#subject-headings)  
- [Labeling and putting stuff away (work in progress)](#labeling-and-putting-stuff-away-work-in-progress)
- [Resources](#resources)

***

# Introduction

![open reel audio in Wilson Library's stacks](https://github.com/annewell/images/blob/main/Stacks_OpenReel.png)
*Open reel audio shelved in Wilson Library's closed stacks.*

Below is documentation related to the arrangement, physical processing, and description of archival, or non-commercial audiovisual (AV) materials. Or rather, this documentation covers AV processing after the point of accession all the way up to access, or finding aid description, and shelving materials in Wilson Library's closed stacks. At this point, this documentaiton page does not cover policies or workflows related to AV conservation, digitization, post-digitization, or quality control (maybe one day?). 

For the most part, archivists physically process and describe AV materials at the item-level to help facilitate preservation via digitization (we're currently developing processes for describing & arranging AV materials at the collection and box-level!...stay tuned.).

In addition to creating finding aid description for AV access, when possible, processing archivists and assistants also enter item-level descriptive metadata of AV items into Jitterbug, an internal online content management system for Wilson Library's analog AV holdings. Jitterbug holds and tracks metadata related to the analog AV format or item ("Audiovisual Items"), as well as metadata related to digitization, including information on the transfer ("Transfers") and the preservation instance or file ("Preservation Instance"). This documentation dives into some Jitterbug specifics related to analog AV items ("Audiovisual Items"), including required metadata fields, field definitions (& style guide), and data entry and import/export methods. 

The outline of this documentation reflects the suggested order of operations for processing analog AV materials: 1. create an arrangmet plan, 2. inventory materials and import or enter item-level metadata into Jitterbug, 3. construct finding aid description using metadata imported or found in Jitterbug, 4. label and shelve materials. 

Please note that this documentation page is a work in progress and will be updated frequently in the summer and fall 2021.

# Arrangement

When assigned an accession containing archival AV materials, consult with a Technical Services archivist about how to best arrange the materials. It is helpful to have an arrangement plan in place before proceeding with item-level processing. Sometimes an arrangement plan is predetermined by the curatorial unit, but often determining an arrangement plan requires some of your own digging and gaining some familiarity with the collection materials. Before diving in, it's helpful to remember that the process of arranging archival AV doesn't vary much from the processes of our manuscript and visual processing colleagues and friends. We often live in a more item-level world when processing AV, but the general methods, practices, and goal of arrangement are the same across formats. The question - how can we best present these materials so people can find what they need? - should guide your approach to arrangment. 

Generally, try to arrange AV materials by content, rather than by format. Exceptions to this may include production-heavy collections with defined works, or titles, that may benefit from having sub-groupings of like-format items in order to gain a sense of the creator's production process. An example of this includes the Tom Davenport Papers, http://finding-aids.lib.unc.edu/20025   

It's also helpful to remember that archival AV items are non-circulating materials. Or rather, access to all archival AV materials requires an intervention of sorts - in-house or external digitization and the production of a viewing or listening copy that is either delivered on physical media to a patron, or more conveniently, is streamed via the online finding aid. This distance grants processing archivists some freedom to present archival AV materials in a meaningful or helpful way in Wilson Library's online finding aids that is not inhibited by the physical materials, which are often stored by like formats across collections and collecting units. In other words, we can present materials intellectually by original order or mixed-format groupings while also storing the materials in preservation friendly groupings and conditions.

Below are examples of arrangement methods of AV materials and when to use them: 

## Original order:

When most of the materials have an existing original order, try to preserve this order. Original order can be identified with curatorial guidance, by obvious or visible original numbering schemes, published discographies, or from supplementary documentation provided by the creator and/or donor. Collections with original order often include record label collections, production-heavy collections with various formats and elements, project based collections, and more generally, collections compiled and organized by the creators themselves. 

**Examples:**

Apollo Records Collection [arranged by record label issue #], http://finding-aids.lib.unc.edu/20539/ 

Peter Lowry Collection [subseries 2.1.1 arranged by the creator's numbering system], http://finding-aids.lib.unc.edu/20017/ 

## Chronological:

If you are dealing primarily with an event or program-based collection, including live performances and radio programs, or a collection that only has materials produced by a single creator, consider using chronological order. Chronological order only works as an arrangement method if most of the items have a date associated with them. If most of the materials in an event/program based or single-creator collection do not have any apparent dates, consider using alphabetical order to group like-events or programs by title.  

**Examples:**

McCabe's Guitar Shop Collection [live shows arranged chronologically by format], http://finding-aids.lib.unc.edu/20511/ 

FolkScene Collection [series 1 consists of radio programs arranged chronologically by production date], http://finding-aids.lib.unc.edu/20517/ 

## Alphabetical:

Use alphabetical order when original order or chronological order are not immediately apparent, or used consistently across the collection. If you are dealing primarily with performer-based recordings, alphabetize by performer’s last name. If you are dealing with event or program-based recordings, alphabetize by program or event titles, when apparent (ex1. Newport Folk Festival, Odetta ; ex2. Newport Folk Festival, Pete Seeger). 

**Examples:**

Greenhill Family/FLi Artists/Folklore Productions Collection [series 3 arranged alphabetically by artist or event], http://finding-aids.lib.unc.edu/20542/ 

# Jitterbug

## Introduction

Once arrangement is determined, consult with the Audiovisual Archivist or Technical Services archivist to decide which method to use to gather and enter item-level metadata into Jitterbug. Jitterbug is accessible to authorized users with an Onyen and Onyen password at the following link: 

https://jitterbug.lib.unc.edu/

![Jitterbug's Audiovisual Items homepage](https://raw.githubusercontent.com/annewell/images/main/Jitterbug_AV_items.PNG)
*Jitterbug’s Audiovisual Items webpage, where metadata relating to the physical AV materials is stored. Note the helpful filters on the left-hand side.*

As mentioned earlier, Jitterbug holds metadata related to the analog AV format or item ("Audiovisual Items"), as well as metadata related to digitization, including information on the transfer ("Transfers") and the preservation instance or file ("Preservation Instance"). This section will cover only the use of the "Audiovisual Items" table, which contains metadata related to the physical item, including format and size, as well as transcribed titles, dates, and locations of production, when known. Audiovisual Items consists of three distinct record types: Audio, Film, and Video. Each record type contains fields specific to that format. It is important to gather all required metadata fields and as many suggested metadata fields as possible during pre-processing work (more on these fields below under [Required fields](#required-fields) and [Suggested fields](#suggested-fields)).

There are 2 options for entering item metadata into Jitterbug – either by creating a new Audio, Film, or Video in the Audiovisual Items table or by creating a CSV file which can then be imported into AV Items. Often the size, or scope, of the collection will determine which data entry method is used. If you just have a handful of items, entering metadata directly into Jitterbug may work best. If you have 50+ items, creating a CSV file for your metadata may be the best method. More on data entry and import below (under [Data Entry and Import](#data-entry-and-import)). 

Before proceeding, it is also a good idea to familiarize yourself with Jitterbug – its fields, search options, and capabilities, such as its auto-generated call numbers, required metadata fields, and suggested metadata fields.  

**Additional jitterbug documentation is located in the departments or G drive: G:\wilson\ts\archival\Jitterbug.** Documentation includes field definitions and style guide ("Jitterbug Field Definitions and Style Guide.xlsx"), as well as a documentation and template related to Jitterbug CSV Items Import (more on that below under Data Entry and Import: [CSV Import](#CSV-import)). 

## Metadata

### Auto-generated call numbers

Call numbers are unique IDs assigned to AV items. They consist of a format specific prefix followed by collection number and item number, "T-4849/1" for example (please note that select Southern Folklife Collection AV materials, like audiotape and audiocassette, have format prefix variations from other collecting units at Wilson - more on format prefixes under [Formats/Container types](#formatscontainer-types)).

Jitterbug’s backend manages or assigns the call number sequences for each collection and its formats. Call numbers should not be manually entered into Jitterbug. If you are creating a record directly in Jitterbug, it will auto-generate an item's call number once the "Collection" and "Format" fields are filled in. If you are importing a CSV, Jitterbug assigns call numbers based on the "Collection" and "Format" fields, as well as the row order of the CSV. It is therefore important to keep the row order in the exact order you wish the call numbers to be assigned by Jitterbug.  
 
PLEASE NOTE that Jitterbug only generates a unique call number once. In other words, if you create a record and delete it, or if you manually change an auto-generated call number, the auto-generated call numbers for that collection will no longer be accurate. 

It is possible to manually change a call number in Jitterbug if a mistake happens, but this change does not update Jitterbug's backend that tells the database which call number to assign next. If you make a mistake (mistakes happen, it's ok!), please consult the Audiovisual Archivist or Technical Services archivist, who will advise on how to proceed. DO NOT delete records unless instructed to. 

### Required fields 

Audiovisual Items records for Audio, Film, and Video items contain required metadata fields, which are listed below by record type. (Spoiler: there are two methods for importing AV Items into Jitterbug, either directly or via CSV import. Please note these differences between these methods in the descriptions below).  
 
AUDIO:   
•	Title: Follow title guidelines found below under "Creating Titles."   
•	Collection: Unique collection ID or number (CSV import) or dropdown list of collection names (Jitterbug interface). Contact the Audiovisual Conservator to add new collection names to the list.  
•	Accession Number: A unique number assigned to an item or group of materials during intake or accession.   
•	Format: Unique format ID (CSV import) or dropdown list of standard audio formats (Jitterbug interface). Consult [Formats/Container types](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#formatscontainer-types) section on this documentation page for more on formats.   
•	Size: Size of audio reel or disc measured in inches.   
 
FILM:   
•	Title: Follow title guidelines found below under "Creating Titles."   
•	Collection: Unique collection ID or number (CSV import) or dropdown list of collection names (Jitterbug interface). Contact the Audiovisual Conservator to add new collection names to the list.  
•	Accession Number: A unique number assigned to an item or group of materials during intake or accession.   
•	Format: Unique format ID (CSV import) or dropdown list of standard film formats (Jitterbug interface). Consult [Formats/Container types](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#formatscontainer-types) section on this documentation page for more on formats.      

VIDEO:   
•	Title: Follow title guidelines found below under "Creating Titles."   
•	Collection: Unique collection ID or number (CSV import) or dropdown list of collection names (Jitterbug interface). Contact the Audiovisual Conservator to add new collection names to the list.  
•	Accession Number: A unique number assigned to an item or group of materials during intake or accession.   
•	Format: Unique format ID (CSV import) or dropdown list of standard video formats (Jitterbug interface). Consult [Formats/Container types](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#formatscontainer-types) section on this documentation page for more on formats.      


### Suggested fields 

Suggested fields are not required, but contain super useful metadata worth gathering when possible. Suggested fields are listed below by Audiovisual Items record type.  
 
AUDIO:   
•	Container Note: Transcription of titles, notes, or memos (such as song titles and performer names) found on or with the item.  
•	Legacy ID: Any number formerly associated with an AV item in this field.   
•	Reel/Tape Number: Extent, or tape number, of recording. (EX: 1/3 ; 2/3 ; 3/3)   
•	Recording Location: Location, or place, of recording.   
•	Access Restrictions: Streaming access restriction determined by curatorial unit.[^1](#endnotes)    
•	Item Year: Catch-all date field that excludes singular full (YYYY-MM-DD) dates.   
•	Item Date: Singular date field formatted as YYYY-MM-DD.   
•	Base: Material that the audio or film item is made of.   

FILM:   
•	Container Note: Transcription of titles, notes, or memos (such as song titles and performer names) found on or with the item.   
•	Legacy ID: Any number formerly associated with an AV item in this field.   
•	Reel/Tape Number: Extent, or tape number, of recording. (EX: 1/3 ; 2/3 ; 3/3)   
•	Recording Location: Location, or place, of recording.   
•	Access Restrictions: Streaming access restriction determined by curatorial unit.[^1](#endnotes)     
•	Item Year: Catch-all date field that excludes singular full (YYYY-MM-DD) dates.   
•	Item Date: Singular date field formatted as YYYY-MM-DD.   
•	Element: A designation of the film formats generation.   
•	Base: Material that the audio or film item is made of.   
•	Color: This field indicates whether a film is color, B/W, or both.    
•	Sound Type: Sound type of film (ex. Optical, Magnetic) with option for "Silent".    
•	Length in Feet: Estimate of the length (in feet) of the film itself.   
 
VIDEO:   
•	Container Note: Transcription of titles, notes, or memos (such as song titles and performer names) found on or with the item.   
•	Legacy ID: Any number formerly associated with an AV item in this field.   
•	Reel/Tape Number: Extent, or tape number, of recording. (EX: 1/3 ; 2/3 ; 3/3)   
•	Recording Location: Location, or place, of recording.   
•	Access Restrictions: Streaming access restriction determined by curatorial unit.[^1](#endnotes)    
•	Item Year: Catch-all date field that excludes singular full (YYYY-MM-DD) dates.   
•	Item Date: Singular date field formatted as YYYY-MM-DD.    

### Field definitions & style guide

No matter which data entry method you choose, how you enter that metadata into Jitterbug’s individual fields remains the same. Please follow the guidelines outlined in the Jitterbug Stylesheet found in the departments or G drive: G:\wilson\ts\archival\Jitterbug\"Jitterbug Field Definitions and Style Guide.xlsx".

Additional guidance on creating item titles can be found below. 

**Creating titles**
Transcribe annotations written on original container into the "Container Note" field in Jitterbug. This field preserves how the title is originally presented on the container. 

If possible, titles include who (performer or event title), what (album or song title), where (recording location using style guide for finding aid [GeogNames](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Style%20Guide.md#geognames)), & when (item year or date using the style guide for finding aid [dates](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Style%20Guide.md#dates)). Below is further guidance on constructing titles: 
 
**Who/What**

    •	Performer, 'Album Title' [single straight quotes '], Date   
        example: Bert Jansch, 'Birthday Blues', 1969 
 
    •	Performer, "Song Title" [double straight quotes "], Date   
        example: Bert Jansch, "Tree Song", 1969 
 
    •	Performer, 'Album Title' or "Song Title", Additional description, Date   
        example: Bert Jansch, 'Birthday Blues', demo, 1968

    •	unidentified performer, "Song Title", Date   
        example: [unidentified artist], "Frosty the Snowman", 12 December 1979

**Only capitalize proper names and titles** (i.e. works, album titles, song titles).  Do not capitalize descriptive words, like "reel", "tape", "demo", "practice", etc.

If a first name is abbreviated (i.e. J. E. Mainer), leave a space between the capitalized letters

If there are multiple items from the same festival/event, place the festival/event name before the performer in the title: 

    •	Festival/Event Name, Performer, Date   
        example: Newport Folk Festival, Muddy Waters, 1967

For studio-based music collection (i.e. Chris Stamey #20562, Duck Kee Studio #20553, Goldband Recording Studio #20245), it is helpful to also add more specific recording details about the recording to the title. Try to stick to the terminology listed on the original container:

    •	dB's, 4-track demos: "Bad Reputation", 1980  
    •	Diesel, practice tape, summer 1975  
    •	Sneakers, rehearsal tape: "Combustion", "Twilight", and "Stimulation", 1 November 1976 

For oral histories, list the subject or interviewee name's first followed by "interview". Also list the interviewer's name if the interviewer is different from the collection’s creator:

    •	Hun Som interview, Greensboro, N.C., 8 June 2003 
    •	Tommy Jarrell interview by Alice Gerrard, Mt. Airy, N.C., 1979   

If a recording or event spans multiple tapes, add the tape number to the title:

    •	Highlander summer camp, 1987, tape 1
    •	Highlander summer camp, 1987, tape 2
    •	Highlander summer camp, 1987, tape 3

Also list the range, if you are certain of the exact range of the materials:
 
    •	Highlander summer camp, 1989, tape 1 of 2
    •	Highlander summer camp, 1989, tape 2 of 2

If an item contains multiple events or recordings, list each event and use a semi-colon to separate events. If multiple locations or dates are listed on a multi-event item, list locations dates in the title using the style guide for finding aid dates:

    •	Beggars, practice tape; Ruby, practice tape 
    •	Peter Holsapple, "Holy Night", September 1985; dB's, "Feliz Navidad", "Holiday Spirit" and "Never Say When"
    •	Dolly Parton, 3 March 1973; Linda Rondstadt, 17 April 1979

If there is no performer or title listed, title the item as an unidentified recording based on the item type: 

    •   [unidentified sound recording]  
    •   [unidentified video recording]  
    •   [unidentified motion picture film]  

If possible, qualify the unidentified recording with the genre/form, and/or a brief description of the contents of the recording. This may only be possible once the recording has been digitized:

    •   [unidentified live performance]  
    •   [unidentified home movie]  
    •   [unidentified Zydeco music]  
    •   [unidentified oral history]  
    •   [unidentified studio recording]  
    •   [unidentified television program]  
 
Place your constructed title into the "Title" field in Jitterbug. Place other pertinent information (Where, When) from container annotations in relevant Jitterbug fields (Recording Location, Item Year, Item Date). 

## Data entry and import

As mentioned above, there are two methods for entering metadata into Jitterbug – either directly into Jitterbug or via csv file import. This section covers steps for both methods.  

### Directly into Jitterbug

1.	After logging in, select "Audio Visual Items" followed by "+ New" 
![Jitterbug webpage with select fields highlighted](https://github.com/annewell/images/blob/main/Jitterbug_dataentry1.PNG)

2.	Select the appropriate record type (Audio, Film, or Video)
![Jitterbug webpage with record type fields highlighted](https://github.com/annewell/images/blob/main/Jitterbug_dataentry2.PNG)

3.	Follow the Jitterbug style guide and enter required metadata fields and as many suggested metadata fields as possible. The Jitterbug style guide can be found in the departments or G drive: G:\wilson\ts\archival\Jitterbug\"Jitterbug Field Definitions and Style Guide.xlsx".

4.	Select "Save", located on the bottom left.   
![Jitterbug webpage with save field highlighted](https://github.com/annewell/images/blob/main/Jitterbug_dataentry3.PNG)

### CSV import

Documentation related to Jitterbug CSV import is located in the departments or G drive: G:\wilson\ts\archival\Jitterbug\"AVitems_import_CSVtemplate". Documentation includes a master spreadsheet of AV format identification numbers, a template for CSV import, and sample CSV import data. 

Below are the steps for creating and importing a CSV import into Jitterbug. The import process can be tedious (hang in there, you got this!).

1.	Open the CSV import template in Open Office and enter required metadata fields and as many suggested metadata fields as possible. We use Open Office since it is opensource and compatible on both Mac and PC, but mostly because it allows us to save the file with the correct encoding (more on that soon). Sample Open Office CSV import data from across collections and accessions illustrated below.  

    ![csv import sample](https://github.com/annewell/images/blob/main/Jitterbug_import_csv.png)

    For larger collections, it may be helpful to inventory the materials upfront. This technique may include assigning temporary IDs with archival paper tape to       each item (as seen below) and then arranging the collection after metadata has been gathered on each item, or simply just keeping materials shelved in the         order you inventoried them. If you choose to add temporary IDs, create a temporary column in your CSV import template to store each item's temporary IDs so       you can match them up with their assigned call number after import.  

    ![temporary IDs on videotapes](https://github.com/annewell/images/blob/main/Jitterbug_tempIDs.png)

2.	Place items in the in the exact row order you wish the call numbers to be assigned by Jitterbug. This order relates to the arrangement plan determined by the pre-processor and Audiovisual Archivist or Technical Services archivist.  
 
    If you assigned temporary IDs to your items, create and save a separate spreadsheet, or labeling guide, with your temporary ID column. Below is an example of     a labeling guide with inventory numbers highlighted in yellow and item call numbers highlighted in green. In this example, call numbers were added to the         labeling guide after arrangement and Jitterbug import to assist with labeling of the materials. 

    ![temporary ID tracking csv](https://github.com/annewell/images/blob/main/Jitterbug_tempIDscsv.png)

3.	Once items are in the correct row order and the temporary ID column has been deleted, select "Save As". Name the file (CollectionNumber_AccessionNumber_import; EX: 20427_107500_import), save the file as a Text CSV (.csv), and select "Edit filter settings" (circled below). Hit Save. 

    ![edit filter settings highlighted](https://github.com/annewell/images/blob/main/Jitterbug_import_settings1.png)

4.	A prompt (illustrated below) may emerge after hitting save. Select "Keep Current Format". 

    ![save settings prompt](https://github.com/annewell/images/blob/main/Jitterbug_import_settings2.png)

5.	Save the file with the following specifications:

    Character set: Unicode (UTF-8)
    Field delimiter (or Separated by): , (comma)
    Text delimiter: "
    select Quote all text cells (or Quoted field as text)
    select Save cell content as shown
    
    PC and MAC file specifications illustrated below:

    ![PC import settings](https://github.com/annewell/images/blob/main/Jitterbug_import_settings3.png)  
    *File specifications from PC version of OpenOffice*  
    
    ![MAC import settings](https://github.com/annewell/images/blob/main/Jitterbug_import_settings4.png)  
    *File specifications from MAC version of OpenOffice*  

6.	Open Jitterbug and on the Audiovisual Items table, select "Batch" --> "Items Import" 

    ![Jitterbug batch import fields highlighted](https://github.com/annewell/images/blob/main/Jitterbug_import_batch.PNG)

7.	Browse for your csv file and select "Upload and Continue" 

    ![Jitterbug batch import pop up window 1](https://github.com/annewell/images/blob/main/Jitterbug_import_batch2.PNG)

8.	Review Items Import and select "Proceed with Import" 

    ![Jitterbug batch import pop up window 1](https://github.com/annewell/images/blob/main/Jitterbug_import_batch3.PNG)

9.  Jitterbug will alert you of any errors with your data (illustrated below in red). If this occurs, fix errors and re-import your csv.  

    ![Jitterbug batch import pop up window 1](https://github.com/annewell/images/blob/main/Jitterbug_import_batch4.PNG)

    Jitterbug will alert you of a successful import.

    Once all the item-level metadata is entered or imported into Jitterbug (YAY!), proceed to # Labeling and Putting Stuff Away (Work in Progress!) below.


## Data export  

Ideally processing archivists create finding aid description for AV materials using an Audio Visual Items metadata export from Jitterbug. 

**To export metadata for an entire collection**, open Audio Visual Items and select the collection name from "Collection Filters" on the left-hand side of the screen, illustrated below. When using filters, make sure you have de-selected other filters, such as "Type Filters" and "Format Filters" - you want to make sure you're getting the entire collection for your export.

![Jitterbug collection filter selected for export](https://github.com/annewell/images/blob/main/Jitterbug_export1.PNG)

**To export a particular accession** from Jitterbug, search the accession number (remember to use quotes!) via the Audio Visual Items search box, illustrated below. As noted above, please be sure to de-select any filters to make sure you are exporting all AV items from an accession.

![Using Jitterbug search function to search accession](https://github.com/annewell/images/blob/main/Jitterbug_export4.PNG)

Once you have the correct collection filter selected or desired accession search results, "Select All" the AV items using the "Ctrl+A" shortcut, and select "Export" via the "Batch" dropdown, illustrated below.

![Jitterbug batch export selected for export](https://github.com/annewell/images/blob/main/Jitterbug_export2.PNG)

When you select "Export" a pop-up window will appear. You can select any appropriate fields you would like to export, or use the "Select All" option, illustrated below, as a quick and easy way to export a collection or accession.

![Jitterbug batch export field options](https://github.com/annewell/images/blob/main/Jitterbug_export3.PNG)

Select the green "Build and Download" button on the bottom of the batch export option and voila!, a csv export, illustrated below, should now be located in your Downloads folder. You can now use this metadata to apply EAD/XML tags discussed further in the [XML/EAD section](#xmlead) below.  

![sample Jitterbug export CSV file](https://github.com/annewell/images/blob/main/Jitterbug_export5.PNG)

# Finding aid description

## Introduction

This section will cover specifics related to finding aid description, including sample XML, container types related to AV items, and a reference section of Library of Congress subject headings that might come in handy when describing AV collections. 

As of June 2021, Technical Services archivists use a Notetab template and hand code XML in Oxygen to create collection finding aids, which are stored in a Github repository (not this one!, a different one :). Archivists follow [DACS descriptive elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Descriptive%20Elements.md) and a local [style guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Style%20Guide.md), which includes information on inclusive description of materials.  

All AV materials are coded at the item-level in finding aids, even materials that span multiple tapes or reels, to facilitate AV digitization and streaming. As mentioned in the introduction on this documentation page, Technical Services archivists are currently exploring other ways to describe AV materials, such as at the collection, series, or box-level. This documentation will be updated as those workflows solidify, but in the meantime this section will stick to workflows related to item-level AV description. This section will not cover broader discussions of finding aid description, such as abstracts, collection titles & dates, etc, which are discussed in both [DACS descriptive elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Descriptive%20Elements.md) and [style guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Style%20Guide.md).

## XML/EAD

To create item-level XML for AV materials, open your CSV export from Jitterbug and isolate fields you would like to call out in description (Call Number, Title, and Format, for example. Some other fields that might be helpful include LegacyID, Reel/TapeNumber, RecordingLocation, ItemYear, ItemDate, and ContentDescription). Create collumns for your XML, illustrated below in green, to properly code your desired metadata.

![sample XML spreadsheet with Jitterbug metadata](https://github.com/annewell/images/blob/main/Description_XMLspreadsheet.PNG)

Once your spreadsheet is complete, you can copy and paste the necessary lines or cells into the collection's XML finding aid.

Below are further suggestions on how to code an AV item at a minimum and moderate level. 

### Minimum (required):

```
<did> 

<container type="container type">Call Number</container> 

<unittitle>Title</unittitle> 

<physdesc> 

<genreform>Format</genreform> 

</physfacet> 

</did> 
```

### Moderate:

```
<did> 

<container type="container type">Call Number</container> 

<unittitle>Title</unittitle> 

<physdesc> 

<genreform>Format</genreform> 

<extent> Reel Size (audio) / Duration (video) / Length in feet (film)</extent> 

</physfacet> 

</did> 
```

Below are examples of how to code an audio, video, and film item when additional information is available. In general, try to keep description at a minimum. 

#### Audio

```
<did> 

<container type="sfcaudioopenreel">Call Number</container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate>: tape number</unittitle>     

<physdesc> 

<genreform>Format</genreform> 

<extent> Reel Size ; Speed ; Duration </extent> 

<physfacet>element type</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - previous numbering schemes, pointing to field notes or related items, playback issues, etc.</p></processinfo> 
```

##### Audio Example:

```
<did> 

<container type="sfcaudioopenreel">FT-20009/1</container> 

<unittitle>Mike and Alice, <geogname>Atlanta, Ga.</geogname>, <unitdate>Date</unitdate>: tape 1 of 2</unittitle>     

<physdesc> 

<genreform>1/4” Open Reel Audio</genreform> 

<extent>5" reel ; 7.5 ips ; 15 minutes, 20 seconds</extent> 

<physfacet>original</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Recording of Mike Seeger and Alice Gerrard performing live.</p> 

</scopecontent> 
```

#### Video

```
<did> 

<container type="videotape">Call Number</container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate>: tape number</unittitle>   

<physdesc> 

<genreform>Format</genreform> 

<extent>Duration</extent> 

<physfacet>element type ; color/black and white ; silent/sound (sound type)</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - previous numbering schemes, pointing to field notes or related items, playback issues, etc.</p></processinfo> 
```

##### Video Example:

```
<did> 

<container type="videotape">VT-20009/1</container> 

<unittitle>Elizabeth Cotton, <geogname>Chapel Hill, N.C.</geogname>, <unitdate>1983</unitdate>: tape 1 of 2</unittitle>   

<physdesc> 

<genreform>Betacam SP</genreform> 

<extent>30 minutes</extent> 

<physfacet>edited master ; color ; sound (mono)</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>An interview with Elizabeth Cotton conducted by Mike Seeger.</p> 

</scopecontent> 

<processinfo><p>Memo found with original container resides in Folder 3</p></processinfo> 
```

#### Film

```
<did> 

<container type="film">Call Number</container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate>: reel number</unittitle> 

<physdesc> 

<genreform>Format</genreform> 

<extent>Length (feet) (Duration)</extent> 

<physfacet>element type ; color/black and white ; silent/sound (sound type)</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - previous numbering schemes, pointing to field notes or related items, playback issues, etc.</p></processinfo> 
```

##### Film Example:

```
<did> 

<container type="film">F-20009/1</container> 

<unittitle>Alice and Hazel, <geogname>Chapel Hill, N.C.</geogname>, <unitdate>1973</unitdate>: reel 1 of 2</unittitle> 

<physdesc> 

<genreform>16mm motion picture film</genreform> 

<extent>800 ft. (25 minutes)</extent> 

<physfacet>reversal ; color ; sound (magnetic)</physfacet>  

</physdesc></did> 

<scopecontent> 

<p>Footage of Alice Gerrard and Hazel Dickens performing live.</p> 

</scopecontent> 
```

#### Born-Digital AV

```
<did> 

<container type="digfolder"> 

<extref href="[insert cdr link]"Call Number</extref></container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate></unittitle> 

<physdesc> 

<extent>Number of files</extent> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - source media, date of original files, note regarding access copies, etc</p></processinfo> 
```

##### Born-Digital Example:

```
<did> 

<container type="digfolder"><extref href="https://cdr.lib.unc.edu/list/uuid:b699afe5-17e3-4020-a55b-a4746c0353f7">DF-20469/1</container> 

<unittitle>Fiddler's Grove Bluegrass Festival, <unitdate>1973</unitdate></unittitle> 

<physdesc> 

<extent>1 digital file</extent> 

</physdesc></did> 

<scopecontent> 

<p>An edited digital version of Brian Burch's Super 8mm footage (F-20469/1-9) set to traditional music. Edited by Brian and Gillen Burch.</p> 

</scopecontent> 

<processinfo><p>Processing information: The digital files were extracted from DVD. Original DVD files are dated 6 July 2005. An access .mp4 file was made from the DVD files for viewing purposes.</p></processinfo> 
```

## Formats/Container types

If you need assistance identifying AV formats, consult the Audiovisual Archivist or a Technical Services archivist. A great online resource for identifying AV is the Preservation Self-Assessment Program's Collection ID Guide: 

https://psap.library.illinois.edu/collection-id-guide 

Below is a guide for AV format description for the Jitterbug database (green), as well as for finding aids (orange). 

### Audio

| Jitterbug Format Display Names | Jitterbug Format ID | SFC Call Number Prefix | SHC / UARMS Call Number Prefix | EAD Container Type(s)                   | Finding Aid < genreform > text                   |
| ------------------------------ | -------------------:| ---------------------- | ------------------------------ | --------------------------------------- | ------------------------------------------------ | 
| Audiocassette                  | 28                  | FS                     | C                              | sfcaudiocassette [FS] audiocassette [C] | Audiocassette                                    | 
| Microcassette                  | 29                  | FS                     | C                              | sfcaudiocassette [FS] audiocassette [C] | Microcassette                                    |
| 8-Track Tape                   | 30                  | 8T                     | ?                              | 8T                                      | 8-Track, tape                                    |
| 1/4" Open Reel Audio           | 31                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | 1/4" open reel audio                             |
| 1/2" Open Reel Audio           | 32                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | 1/2" open reel audio                             |
| 1" Open Reel Audio             | 33                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | 1" open reel audio                               |
| 2" Open Reel Audio             | 34                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | 2" open reel audio                               |
| ADAT                           | 35                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | Alesis Digital Audio Tape (ADAT)                 |
| Digital Audio Tape (DAT)       | 36                  | DAT                    | DAT                            | dat                                     | Digital Audio Tape (DAT)                         |
| Hi8 (Audio Tape)               | 37                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | Hi8 [Audio]                                      |
| Data8                          | 38                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | Data8                                            |
| U-Matic (Audio Tape)           | 39                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | U-Matic [Audio]                                  |
| Beta (PCM-F1)                  | 40                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | Beta (PCM-F1) [Audio]                            |
| VHS (PCM-F1)                   | 41                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | VHS (PCM-F1) [Audio]                             |
| Instantaneous Disc             | 45                  | FD                     | FD (legacy: D)                          | fd                                      | Acetate disc / Lacquer disc / Instantaneous disc |
| Transcription Disc             | 46                  | TR                     | TR (legacy: D)                          | trans                                   | Transcription disc                               |
| Wire Recording                 | 47                  | WR                     | WR                             | wr                                      | Wire recording                                   |
| 45                             | 48                  | 45                     | 45 (legacy: D)                           | audiodisc                               | 45-rpm record                                    |
| 78                             | 49                  | 78                     | 78 (legacy: D)                           | audiodisc                               | 78-rpm record                                    |
| Cylinder                       | 50                  | CY                     | CY                             | ?                                       | Cylinder                                         |
| MiniDisc                       | 51                  | MD                     | MD                             | md                                      | MiniDisc                                         |
| LP                             | 52                  | FC                     | FC (legacy: D)                          | audiodisc                               | LP record                                        |
| Flexi Disc                     | 53                  | FC                     | FC (legacy: D)                        | audiodisc                               | Flexi disc                                       |
| Analog Disc                    | 54                  | D                      | D                        | audiodisc                               | Metal stamper                                    |
| NAB Catridge                   | 56                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | NAB cartridge                                    |

### Video

| Jitterbug Format Display Names | Jitterbug Format ID | SFC Call Number Prefix | SHC / UARMS Call Number Prefix | EAD Container Type(s) | Finding Aid < genreform > text |
| ------------------------------ | -------------------:| ---------------------- | ------------------------------ | --------------------- | ------------------------------ | 
| Betacam                        | 7                   | VT                     | VT                             | videotape             | Betacam                        | 
| Betacam SP                     | 8                   | VT                     | VT                             | videotape             | Betacam SP                     |
| Betamax                        | 9                   | VT                     | VT                             | videotape             | Betamax                        |
| U-Matic                        | 10                  | VT                     | VT                             | videotape             | U-Matic                        |
| U-Matic SP                     | 11                  | VT                     | VT                             | videotape             | U-Matic SP                     |
| VHS                            | 12                  | VT                     | VT                             | videotape             | VHS / VHS-C / S-VHS            |
| HDCAM                          | 13                  | VT                     | VT                             | videotape             | HDCAM                          |
| DVCAM                          | 14                  | VT                     | VT                             | videotape             | DVCAM                          |
| MiniDV                         | 15                  | VT                     | VT                             | videotape             | MiniDV                         |
| Digital Betacam                | 16                  | VT                     | VT                             | videotape             | Digital Betacam                |
| Hi8                            | 17                  | VT                     | VT                             | videotape             | Hi-8                           |
| Video8                         | 18                  | VT                     | VT                             | videotape             | Video8                         |
| Digital 8                      | 19                  | VT                     | VT                             | videotape             | Digital 8                      |
| D-2                            | 20                  | VT                     | VT                             | videotape             | D-2                            |
| M-Format                       | 21                  | VT                     | VT                             | videotape             | M-Format                       |
| 2" Open Reel Video             | 22                  | VT                     | VT                             | videotape             | 2" open reel video             |
| 1" Open Reel Video             | 23                  | VT                     | VT                             | videotape             | 1" open reel video             |
| 1/2" Open Reel Video           | 24                  | VT                     | VT                             | videotape             | 1/2" open reel video           |

### Film

| Jitterbug Format Display Names | Jitterbug Format ID | SFC Call Number Prefix | SHC / UARMS Call Number Prefix | EAD Container Type(s) | Finding Aid < genreform > text |
| ------------------------------ | -------------------:| ---------------------- | ------------------------------ | --------------------- | ------------------------------ | 
| 35mm                           | 1                   | F                      | F                              | film                  | 35mm motion picture film       | 
| 16mm                           | 2                   | F                      | F                              | film                  | 16mm motion picture film       |
| Super 8mm                      | 3                   | F                      | F                              | film                  | Super 8mm motion picture film  |
| 8mm                            | 4                   | F                      | F                              | film                  | 8mm motion picture film        |
| 9.5mm                          | 5                   | F                      | F                              | film                  | 9.5mm motion picture film      |
| Filmstrip                      | 6                   | F                      | F                              | film                  | Filmstrip                      |
| Film preservation instance     | 6                   | FPI                    | FPI                              | fpi                   | 16mm motion picture film preservation instance         | 

## Subject headings

A great resource for folklore soud recording collections is the **American Folklore Society's Ethnographic Thesaurus:** http://id.loc.gov/vocabulary/ethnographicTerms.html 

Listed below is a local controlled vocabulary for music-based and/or AV centric collections. Subject headings are arranged loosely by genre or subject. For more widely applicable subject terms (i.e.: Folk music., Folk songs., Dance music., etc), it may be useful to further specify the heading with a geographic location (i.e. Folk music--North Carolina.).  

#### Blues and R&B:

- Blues (Music)
- Blues musicians.
- Doo-wop (Music)
- Harmonica music.
- Piedmont blues.
- Popular muisc--United States.
- Rhythm and blues music.

#### Country western:

- Country dance.
- Country music.
- Country western swing.
- Country music festivals.
- Cowboys-- Songs and music.
- West (U.S.)--Songs and music.
- Western films.

#### Folk, Old-time, and Bluegrass:

- Ballads, English--Southern States.  
- Ballads, English--North Carolina. 
- Ballads, English--Texts. 
- Banjo music.  
- Bluegrass music. 
- Dance music--North Carolina. 
- Dulcimer music. 
- Fiddle contests.
- Fiddle festivals.
- Fiddle tunes--Southern States. 
- Fiddlers. 
- Field recordings--North Carolina. 
- Folk dance music--North Carolina. 
- Folk festivals--North Carolina. 
- Folk music--North Carolina. 
- Folk music--Virginia. 
- Folk music--West Virginia. 
- Folk musicians--North Carolina. 
- Folk songs, English--North Carolina. 
- Folk songs, English -- United States. 
- Folklore--North Carolina.  
- Guitar music--North Carolina.  
- Hymns, English--North Carolina 
- Old-time music--Southern States.  

#### Radio recordings:

- Radio broadcasting--United States.  
- Radio programs--United States. 
- Radio programs, Musical--United States. 
- Documentary radio programs. 
- Radio airchecks. 
- Radio employees. 
- Radio interviews. 
- Radio outtakes. 
- Radio scripts. 
- Radio serials. 

#### Religious recordings:

- African American churches--North Carolina. 
- African Methodist Episcopal Zion Church.  
- Baptists--Hymns.
- Church services--North Carolina. 
- Church choirs--North Carolina. 
- Church music--North Carolina. 
- Divination--North Carolina.
- Funeral rites and ceremonies--United States.
- Funeral service.
- Hymns, English--North Carolina. 
- Gospel music--North Carolina.
- Primitive Baptists--Clergy--North Carolina. 
- Prayer--North Carolina. 
- Preaching--North Carolina. 
- Primitive Baptists--Hymns. 
- Primitive Baptists--North Carolina. 
- Primitive Baptists--Virginia.  
- Proverbs--North Carolina.  
- Regular Baptists--Kentucky.
- Religious life and customs--North Carolina. 
- Religious life and customs--Virginia. 
- Religious practices—North Carolina.  
- Sacred music--North Carolina. 
- Sermons, American--North Carolina. 
- Spirituals (Songs)--North Carolina. 

#### Oral History interviews and storytelling:

- Oral histories.
- Storytellers--South Carolina.
- Storytelling--South Carolina.
- Tales--Southern States.

#### Folk art:

- Artists--North Carolina. 
- Boatbuilders--North Carolina. 
- Chair-makers--North Carolina. 
- Folk art--North Carolina. 
- Folk art museums--North Carolina. 
- Folk artists--North Carolina. 
- Hand weaving--North Carolina. 
- North Carolina Folk Heritage Award. 
- Painters--North Carolina. 
- Painting, American--North Carolina. 
- Potters--North Carolina. 
- Pottery, American--North Carolina. 
- Quilts--North Carolina. 
- Quilting--North Carolina. 
- Sculptors--North Carolina. 
- Sculpture, American--North Carolina. 
- Self-taught artists--North Carolina. 
- Ship models--North Carolina. 
- Weavers--North Carolina. 
- Weaving--North Carolina. 

#### Protest Music/Art:

- Civil rights movements--Southern States. 
- Protest--North Carolina 
- Protest art--North Carolina. 
- Protest demonstrations--North Carolina. 
- Protest marches--North Carolina. 
- Protest songs--Southern States. 
- Work songs--Southern States. 

# Labeling and putting stuff away (work in progress!)

_This section is a work in progress...stay tuned!_

## Rehousing Materials

Apart from moving image film, it is preferable to leave AV materials in their original containers since these containers often contain information about the original stock, as well as container notes created by the creator or donor of the collection. Exceptions to this include original containers with severe preservation or conservation concerns, such as mold or an inability to properly contain the item at hand.  

Whenever an AV material is rehoused, transcribe all titles and container notes from the original container into Jitterbug and photocopy or digitally photograph the original container. Place the photocopy or photograph in the collection’s control file or the curatorial unit's Department Drive until proper procedures for documenting original containers are developed.  

Unlike audio and video formats, all moving image film is hand inspected, placed onto archival cores, and rehoused into archival cans. Consult the Audiovisual Archivist about film inspection and rehousing before proceeding with moving image materials.  

## Labeling

#### Create small item labels

Once you have retrieved the correct call numbers, see “How to Create Item level AV Labels.docx” (_Louis\Southern Folklife Collection\Departmental Documents\Documentation\Archival Processing \How to Create Item Level AV Labels.docx_) and create labels using foil-back spine labels supplied by Technical Services. 

#### Physically label items

Labels for cartridge-based items, such as audiocassettes and videotape, are placed on the spine, while labels for open reel and audiodiscs, are placed on the top left front of the item. Mail merge templates for both spine ("AV_spine_labels.docx") and front-facing ("AV_front_labels.docx") labels reside in the departments drive (G:\wilson\sfc\LABELS\Anne). Labels for moving image film are created with the label maker located on level 10. More on label type and placement below.  

ADD PICTURES HERE

#### Cartridge-based item labels

When possible for cartridge-based items, place item labels on the spine of the container. 

ADD PICTURES HERE

## Boxing AV

Small to medium-sized AV materials require additional housing into archival boxes. Larger formats that do not require additional housing include: 

#### Audio:

- ¼” Open Reel Audio 
- ½” Open Reel Audio 
- 1” Open Reel Audio 
- 2” Open Reel Audio 

Videotape formats used as audio, such as ADAT and VHS (PCM-F1)

#### Motion Picutre Film:

- 35mm 
- 16mm 
- Super 8mm 
- 8mm 
- 9.5mm
- Filmstrips

#### Videotape:

- ½” Open Reel Video 
- 1” Open Reel Video 
- 2” Open Reel Video

The small to medium-sized AV materials AV formats that do require additional housing into archival boxes are listed below with the appropriate box title and box type: 

#### Audio:

| Box Title                 | Format(s)                     | Box Type               |
| ------------------------- | ----------------------------- | ---------------------- |
| 8-Track Tapes             | 8-Track tape                  | Archival CD            |
| Audiocassettes            | Audiocassette; Microcassettes | Archival Audiocassette |
| Digital Audio Tapes (DAT) | DAT                           | Archival Audiocassette |
| MiniDiscs                 | MiniDisc                      | Archival Audiocassette |
| Transcription Discs       | Transcription Discs           | Transcription Disc     |
| Instantaneous Discs       | Instantaneous Discs           | Instantaneous Disc     |

#### Video:

| Box Title         | Format(s)                                                                  | Box Type               |
| ----------------- | -------------------------------------------------------------------------- | ---------------------- |
| Videotape | Betacam; Betacam SP; Betamax; Digital Betacam; U-Matic; VHS; D-2; M-Format; VHS-C; HDCAM; DVCAM; MiniDV; Hi8; Video8; Digital 8 | Paige Box              |

Please note existing labels for shared AV boxes, such as "Videotape box", "Audiocassette box", etc, are stored in the file folder located in TS archival's processing room.


# Resources  

This documentaiton page did not emerge from a vacuum! As the Audiovisual Archivist at Wilson Library, I lean on and acknowledge the many smart & thoughtful people who have presented and published widely on the subject of processing archival AV materials. Below is a growing & ever-evolving list of some recommended resources to check out if you haven't already:

- University of Illinois at Urbana-Champaign's [Preservation Self-Assessment Program: "Collection ID Guide: Audiovisual Materials"](https://psap.library.illinois.edu/collection-id-guide#audiovisual)

a great resource (with lots of photographs) for identifying analog audiovisual formats. 

- Megan McShea, Smithsonian Archives of American Art, ["Guidelines for processing archival collections with audiovisual material"](https://www.aaa.si.edu/tags/documentation)

a thorough and thoughtful approach to processing archival audiovisual materials in a finding aid context.

- New York University Libraries, ["Descriptive Policies on Audiovisual and Born-digital Materials"](https://docs.google.com/document/d/1Zcvp57201jEgsGZgT8Up1c7nIWAwdtHHBMZn3NYogRs/edit)

a peek at another academic instutition's documentation on descriptive policies for audiovisual and born-digital materials (thank you NYU folks!).

# Endnotes

^1 item-level streaming access restrictions ("Open", "Campus", or "Closed") are determined by the curatorial unit. Access restrictions are ideally determined during intake or acquisition. Processing Archivists may need to correspond with the curatorial unit to gather additional item-level restrictions.  


