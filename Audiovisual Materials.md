Content owner: **Anne Wells**

Updated January 2022 by Anne Wells.

# Overview
- [Introduction](#introduction)
- [Processing levels](#processing-levels)
- [Arrangement](#arrangement)
- [Jitterbug](#jitterbug)  
    -[Metadata](#metadata)  (call numbers, required & suggested fields, field definitions & style guide, creating titles)  
    -[Data entry and import](#data-entry-and-import)  
    -[Data export](#data-export) 
- [Finding aid description](#finding-aid-description)  
    -[Formats/container types](#formatscontainer-types)  
    -[XML/EAD](#xmlead)  
    -[LC Subject Headings](#subject-headings)  
- [Labeling and putting stuff away](#labeling-and-putting-stuff-away)  
    -[Rehousing](#rehousing-materials)      
    -[AV item labels](#av-item-labels)    
    -[AV box types and labels](#av-box-types-and-labels)      
    -[Shelving](#shelving)    
    -[Creating locations in ASpace](#creating-locations-in-archivesspace)    
- [Resources](#resources)

***

# Introduction

![open reel audio in Wilson Library's stacks](https://github.com/annewell/images/blob/main/Stacks_OpenReel.png)
*Open reel audio shelved in Wilson Library's closed stacks.*

Below is documentation related to the arrangement, physical processing, and description of archival, or non-commercial audiovisual (AV) materials. These materials include analog audio or sound recordings, video tapes, and motion picture films, as well as born-digial AV materials that originate in digital form. 

This documentation covers AV processing after the point of accessioning all the way up to access, or finding aid description, and shelving materials in Wilson Library's closed stacks. At this point, this documentation page does not cover policies or workflows related to AV conservation, digitization, post-digitization, or quality control (maybe one day?). 

For the most part, Technical Services processing archivists physically process and describe AV materials at the item-level to help facilitate preservation via digitization and straemable access via a finding aid. Technical Services is currently developing processes for describing & arranging AV materials at other processing levels, including collection and box-level description...stay tuned.

In addition to creating finding aid description for AV access, when possible, processing archivists and assistants also enter item-level descriptive metadata of AV items into Jitterbug, an internal online content management system for Wilson Library's analog AV holdings. Jitterbug holds and tracks metadata related to the analog AV format or item ("Audiovisual Items"), as well as metadata related to digitization, including information on the transfer ("Transfers") and the preservation instance or file ("Preservation Instance"). This documentation dives into some Jitterbug specifics related to analog AV items ("Audiovisual Items"), including required metadata fields, field definitions (& style guide), and data entry and import/export methods. 

The outline of this documentation reflects the suggested order of operations for processing analog AV materials: 1. create an arrangement plan, 2. inventory materials and import or enter item-level metadata into Jitterbug, 3. construct finding aid description using metadata imported or found in Jitterbug, 4. label and shelve materials. But before we get to all that, let's talk processing levels (continue below).

Please note that this documentation page is a work in progress and will be updated frequently in 2022.

# Processing Levels

Like manuscript or paper materials, archival AV items can be processed at various states or levels that are informed by available resources and shared library-wide priorities and values: [Intensive (item-level processing)](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#intensive-item-level-processing); [Moderate (box-level processing)](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#moderate-box-level-processing); and [Minimum (collection-level processing)](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#minimum-collection-level-processing)

During the multi-phase [Andrew W. Mellon funded grant project](https://library.unc.edu/wilson/sfc/audiovisual-preservation/), grant-funded staff focused primarily on very intensive item-level processing of AV materials to help facilitate digitization for preservation and access purposes...hence most of this documentation page being **VERY** item-level focused. The grant-funded team did such intensive processing of AV items because there was funding and staff (shout out to the amazing AV conservator, audio engineers, AV Assistants, Graduate Assistants, Grant PIs, and me, the AV Archivist!), but this project is coming to a close, and reality is setting in – how can this intensive and highly specialized work continue at Wilson Library? Below is some guidance on how to handle archival AV items based on resources, priorities, and values.  

## Intensive (item-level processing)

As mentioned, this documentation site primarily covers item-level processing of AV materials, which includes creating an arrangement plan, entering, or importing item-level metadata into Jitterbug, and adding item-level to description to finding aids based on Technical Services' style guide. 

I think a simple way to think of when such intensive work is necessary is based on whether an AV item requires a call number after accessioning – either for digitization or finding aid access. What would trigger this? Great question 😊 : perhaps materials or collections that align with [The Reckoning Initiative at the University Libraries](https://library.unc.edu/reckoning/); to facilitate access for research-driven requests; or maybe work related to special projects based on other library-wide priorities and values.

Below is a brief overview of what is required at the intensive processing level. 

### Pre-Processing

Processing Archivists and/or Graduate Assistants conceptualize an arrangement plan for materials (see [Arrangement](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#arrangement)) and create item-level metadata for each AV item based on this plan. This AV item metadata is entered or imported into Jitterbug (see [Jitterbug](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#jitterbug)). Each AV item is labeled and shelved on level 10 in the appropriate location (see [Labeling and putting stuff away](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#labeling-and-putting-stuff-away)).

### Description

Processing Archivists export item-level metadata from Jitterbug (see [Data export](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#data-export)) and create item-level description of materials based on Technical Services' [Style Guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Style%20Guide.md) and the [XML/EAD section](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#xmlead) found on this documentation page. 
### Locations

When AV items are described at the item-level in the finding aid, Processing Archivists assign locations for each item or range of items to the appropriate Resource record in ArchivesSpace (see [Creating locations in ASpace](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#creating-locations-in-archivesspace)).

If the AV materials you have require a call number or intensive item-level work, proceed to the next section, [Arrangement](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#arrangement). If you’re curious about other processing levels, please keep reading.

## Moderate (box-level processing)

If a large AV collection comes in and has clear or obvious groupings, such as AV items by different creators (artist, performer, or musical group) and/or AV items related to multiple projects, works, or labels, it may be helpful to both researchers and front-facing library staff for Technical Services' archivists to conduct a rough arrangement and description of materials to help facilitate mediated access to the collection. 

Below is a brief overview of what is required at this moderate processing level. 

### Pre-Processing

Place like AV items or groupings in archival boxes or paige boxes, and number or label these boxes, using the standard document cartons/document case label but with the added “AV prefix: AV Box 1, AV Box 2, AV Box 3, etc. (see [Labeling and putting stuff away](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#labeling-and-putting-stuff-away)).

### Description

Describe AV items at the box-level in the finding aid with the EAD container type "avbox" and appropriate box number and unit title description. Boxes can be listed or described individually or in ranges – whatever is appropriate for the materials. It may also be helpful to roughly describe the materials in the scope and content note (see [XML/EAD](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#av-box) for examples). 

Assign the appropriate access restriction at the series and collection levels so that researchers understand AV items may require further processing to be accessed and/or digitized. 

### Locations

If boxes are described in the finding aid, assign box location(s) to the appropriate collection Resource record in ArchivesSpace. Select "AV Box" as the child type and the appropriate box number as the child indicator (see [Creating locations in ASpace](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#creating-locations-in-archivesspace)).

## Minimum (collection-level processing)

Collection level records for unprocessed materials contain the elements prescribed by DACS for a single-level minimum record (see Technical Services' [Collection Level Records](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Collection-Level-Records.md) page for more). The majority of new accessions at Wilson Library will receive this treatment to facilitate quick medicated access to collection materials. If a researcher is interested in using materials described in a collection-level collection, further processing, such as box or item-level, may take place.

Below is a brief overview of what is required at this minimum processing level: 

### Pre-Processing

Place AV items in archival boxes or paige boxes, and number or label these boxes, using the standard document cartons/document case label but with the added AV prefix: AV Box 1, AV Box 2, AV Box 3, etc. (see [Labeling and putting stuff away](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#labeling-and-putting-stuff-away)). It's not required or necessary to arrange AV items at this time, but if easy categories or groupings emerge, why not 😊? You'll be helping your colleague who picks up this collection next.

### Description

Describe AV items in the collection abstract when appropriate. Assign the appropriate access restriction at the collection level so that researchers understand AV items require further processing to be accessed and/or digitized.  (Yep, that's it! Easy.)

### Locations

Assign box location(s) to the appropriate Accession record in ArchivesSpace. Select "AV Box" as the child type and the appropriate box number as the child indicator (see [Creating locations in ASpace](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#creating-locations-in-archivesspace)).

Now onto arrangement.

# Arrangement

When assigned an accession containing archival AV materials, consult with a Technical Services archivist about how to best arrange the materials. It is helpful to have an arrangement plan in place before proceeding with item-level processing. Sometimes an arrangement plan is predetermined by the curatorial unit or by previously arranged accessions from the collection, but often determining an arrangement plan requires some of your own digging and gaining some familiarity with the collection materials. Before diving in, check to see if there is an existing finding aid for the collection to see if there is already an arrangement plan in place. It's also helpful to remember that the process of arranging archival AV doesn't vary much from the processes of our manuscript and visual processing colleagues and friends. We often live in a more item-level world when processing AV, but the general methods, practices, and goal of arrangement are the same across formats. The question - how can we best present these materials so people can find what they need? - should guide your approach to arrangement. 

Generally, try to arrange AV materials by content, rather than by format. Exceptions to this may include production-heavy collections with defined works, or titles, that may benefit from having sub-groupings of like-format items to gain a sense of the creator's production process. An example of this includes the Tom Davenport Papers, http://finding-aids.lib.unc.edu/20025   

It's also helpful to remember that archival AV items are non-circulating materials. Or rather, access to all archival AV materials requires an intervention of sorts - in-house or external digitization and the production of a viewing or listening copy that is either delivered on physical media to a patron, or more conveniently, is streamed via the online finding aid. This distance grants processing archivists some freedom to present archival AV materials in a meaningful or helpful way in Wilson Library's online finding aids that is not inhibited by the physical materials, which are often stored by like formats across collections and collecting units. In other words, we can present materials intellectually by original order or mixed-format groupings while also storing the materials in preservation friendly groupings and conditions.

Below are examples of arrangement methods of AV materials and when to use them: 

## Original order:

When most of the materials have an existing original order, try to preserve this order. Original order can be identified with curatorial guidance, by obvious or visible original numbering schemes, published discographies, or from supplementary documentation provided by the creator and/or donor. Collections with original order often include record label collections, production-heavy collections with various formats and elements, project-based collections, and more generally, collections compiled and organized by the creators themselves. 

**Examples:**

Apollo Records Collection [arranged by record label issue #], http://finding-aids.lib.unc.edu/20539/ 

Peter Lowry Collection [subseries 2.1.1 arranged by the creator's numbering system], http://finding-aids.lib.unc.edu/20017/ 

## Chronological:

If you are dealing primarily with an event or program-based collection, including live performances and radio programs, or a collection that only has materials produced by a single creator, consider using chronological order. Chronological order only works as an arrangement method if most of the items have a date associated with them. If most of the materials in an event/program based or single-creator collection do not have any apparent dates, consider using alphabetical order to group like-events or programs by title.  

**Examples:**

McCabe's Guitar Shop Collection [live shows arranged chronologically by format], http://finding-aids.lib.unc.edu/20511/ 

FolkScene Collection [series 1 consists of radio programs arranged chronologically by production date], http://finding-aids.lib.unc.edu/20517/ 

## Alphabetical:

Use alphabetical order when original order or chronological order are not immediately apparent or used consistently across the collection. If you are dealing primarily with performer-based recordings, alphabetize by performer’s last name. If you are dealing with event or program-based recordings, alphabetize by program or event titles, when apparent (ex1. Newport Folk Festival, Odetta ; ex2. Newport Folk Festival, Pete Seeger). 

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

### Call numbers

Call numbers are unique IDs assigned to AV items. They consist of a format specific prefix followed by collection number and item number ("T-4849/1" for example). Please note that select Southern Folklife Collection AV items, like audiotape and audiocassette, have different format prefixes from other collecting units at Wilson - more on format prefixes under [Formats/Container types](#formatscontainer-types)). 

To make things even more fun, Southern Folklife Collection AV items may have either one of two call number types - a. the one mentioned above, a format specific prefix followed by collection number and item number ("FS-20511/1" for example), or a legacy numbering system that consists of consecutively numbered items that span across SFC collections (FS-16012, FS-16013, FS-16014, and so on, for example). For the most part, with new accessions you will probably be encountering the "collection slash" call number type, as I like to call it. The good news, is that you don't need to know which style of call numbers to assign to SFC AV items (collection slash or legacy style), because Jitterbug does this work for you - more on that below under Auto-generated call numbers. The kind of bad news is that these two call number types have their own unique boxing and shelving workflows - more on that in [Labeling and putting stuff away](#labeling-and-putting-stuff-away-work-in-progress) section of this documentation.

**Auto-generated call numbers**:

Jitterbug’s backend manages or assigns the call number sequences for each collection and its formats. **Call numbers should not be manually entered into Jitterbug.** If you are creating a record directly in Jitterbug, it will auto-generate an item's call number once the "Collection" and "Format" fields are filled in. If you are importing a CSV, Jitterbug assigns call numbers based on the "Collection" and "Format" fields, as well as the row order of the CSV. It is therefore super important to keep the row order in the exact order you wish the call numbers to be assigned by Jitterbug.  
 
PLEASE NOTE that Jitterbug only generates a unique call number once. In other words, if you create a record and delete it, or if you manually change an auto-generated call number, the auto-generated call numbers for that collection will no longer be accurate. 

It is possible to manually change a call number in Jitterbug if a mistake happens, but this change does not update Jitterbug's backend that tells the database which call number to assign next. If you make a mistake (mistakes happen, it's ok!), please consult the Audiovisual Archivist or Technical Services archivist, who will advise on how to proceed. **DO NOT delete records unless instructed to.** 

### Required fields 

Audio Visual Items records for Audio, Film, and Video items contain required metadata fields, which are listed below by record type.  
 
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

Suggested fields are not required but contain super useful metadata worth gathering when possible. Suggested fields are listed below by Audiovisual Items record type.  
 
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

### Creating titles  
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

Also list the range if you are certain of the exact range of the materials:
 
    •	Highlander summer camp, 1989, tape 1 of 2
    •	Highlander summer camp, 1989, tape 2 of 2

If an item contains multiple events or recordings, list each event and use a semi-colon to separate events. If multiple locations or dates are listed on a multi-event item list locations dates in the title using the style guide for finding aid dates:

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

Documentation related to Jitterbug CSV import is located in the departments or G drive: 

**G:\wilson\ts\archival\Jitterbug\"AVitems_import_CSVtemplate"**

Documentation includes a master spreadsheet of AV format identification numbers, a template for CSV import, and sample CSV import data. 

Below are the steps for creating and importing a CSV import into Jitterbug. The import process can be tedious (hang in there, you got this!).

1.	Open the CSV import template in Open Office (download here: https://www.openoffice.org/) and enter required metadata fields and as many suggested metadata fields as possible. We use Open Office since it is opensource and compatible on both Mac and PC, but mostly because it allows us to save the file with the correct encoding (more on that soon). Sample Open Office CSV import data from across collections and accessions illustrated below.  

    ![csv import sample](https://github.com/annewell/images/blob/main/Jitterbug_import_csv.png)

    For larger collections, it may be helpful to inventory the materials upfront. This technique may include assigning temporary IDs with archival paper tape to       each item (as seen below) and then arranging the collection after metadata has been gathered on each item, or simply just keeping materials shelved in the         order you inventoried them. If you choose to add temporary IDs, create a temporary column in your CSV import template to store each item's temporary IDs so       you can match them up with their assigned call number after import.  

    ![temporary IDs on videotapes](https://github.com/annewell/images/blob/main/Jitterbug_tempIDs.png)

2.	Place items in the in the exact row order you wish the call numbers to be assigned by Jitterbug. This order relates to the arrangement plan determined by the pre-processor and Audiovisual Archivist or Technical Services archivist.  
 
    If you assigned temporary IDs to your items create and save a separate spreadsheet, or labeling guide, with your temporary ID column. Below is an example of     a labeling guide with inventory numbers highlighted in yellow and item call numbers highlighted in green. In this example, call numbers were added to the         labeling guide after arrangement and Jitterbug import to assist with labeling of the materials. 

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

    If you are pre-processing materials and NOT working on finding aid description, proceed to [Labeling and Putting Stuff Away](#labeling-and-putting-stuff-away) once all the item-level metadata is entered or imported into Jitterbug (YAY!).


## Data export  

Ideally Technical Services archivists create finding aid description for AV materials using an Audio Visual Items metadata export from Jitterbug. 

**To export metadata for an entire collection**, open Audio Visual Items and select the collection name from "Collection Filters" on the left-hand side of the screen, illustrated below. When using filters, make sure you have de-selected other filters, such as "Type Filters" and "Format Filters" - you want to make sure you're getting the entire collection for your export.

![Jitterbug collection filter selected for export](https://github.com/annewell/images/blob/main/Jitterbug_export1.PNG)

**To export a particular accession** from Jitterbug, search the accession number (remember to use quotes!) via the Audio Visual Items search box, illustrated below. As noted above, please be sure to de-select any filters to make sure you are exporting all AV items from an accession.

![Using Jitterbug search function to search accession](https://github.com/annewell/images/blob/main/Jitterbug_export4.PNG)

Once you have the correct collection filter selected or desired accession search results "Select All" the AV items using the "Ctrl+A" shortcut and select "Export" via the "Batch" dropdown, illustrated below.

![Jitterbug batch export selected for export](https://github.com/annewell/images/blob/main/Jitterbug_export2.PNG)

When you select "Export" a pop-up window will appear. You can select any appropriate fields you would like to export, or use the "Select All" option, illustrated below, as a quick and easy way to export a collection or accession.

![Jitterbug batch export field options](https://github.com/annewell/images/blob/main/Jitterbug_export3.PNG)

Select the green "Build and Download" button on the bottom of the batch export option and voila!, a csv export, illustrated below, should now be in your Downloads folder. You can now use this metadata to apply EAD/XML tags discussed further in the [XML/EAD section](#xmlead) below.  

![sample Jitterbug export CSV file](https://github.com/annewell/images/blob/main/Jitterbug_export5.PNG)

# Finding aid description

## Introduction

This section will cover specifics related to finding aid description, including sample XML, container types related to AV items, and a reference section of Library of Congress subject headings that might come in handy when describing AV collections. 

As of June 2021, Technical Services archivists are the only folks creating and publishing finding aid description. TS archivists use a Notetab template and hand code XML in Oxygen to create collection finding aids, which are stored in a Github repository (not this one!, a different one :). Archivists follow [DACS descriptive elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Descriptive%20Elements.md) and a local [style guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Style%20Guide.md), which includes information on inclusive description of materials.  

All AV materials are coded at the item-level in finding aids, even materials that span multiple tapes or reels, to facilitate AV digitization and streaming. As mentioned in the introduction on this documentation page, Technical Services archivists are currently exploring other ways to describe AV materials, such as at the collection, series, or box-level. This documentation will be updated as those workflows solidify, but in the meantime this section will stick to workflows related to item-level AV description. This section will not cover broader discussions of finding aid description, such as abstracts, collection titles & dates, etc, which are discussed in both [DACS descriptive elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Descriptive%20Elements.md) and [style guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Style%20Guide.md).

## XML/EAD

To create item-level XML for AV materials, open your CSV export from Jitterbug and isolate fields you would like to call out in description (Call Number, Title, and Format, for example. Some other fields that might be helpful include LegacyID, Reel/TapeNumber, RecordingLocation, ItemYear, ItemDate, and ContentDescription). 

Create columns for your XML, illustrated below in green, to properly code your desired metadata:

![sample XML spreadsheet with Jitterbug metadata](https://github.com/annewell/images/blob/main/Description_XMLspreadsheet.PNG)

Some examples of spreadsheet coding below:

```
<c03><did><container type="videotape">VT-5773/104</container><unittitle>Enduring Voices Project, Interview of Mr. Robert Bushyhead, copy, 2 November 1997</unittitle><physdesc><genreform>VHS</genreform></physdesc></did></c03>

<c02><did><container type="audiotape">T-70092/5</container><unittitle>WAFR: Black Seeds: Angela Davis and Helen Othow Interview, 1974</unittitle><physdesc><genreform>1/4" Open Reel Audio</genreform></physdesc></did><processinfo><p>Original number: SOHP0257</p></processinfo><scopecontent><p>Description from inventory: Host - Julius Blakely, Guests - Angela Davis and Helen Othow; Julius Blakely interviews Angela Davis and Helen Othow.</p></scopecontent></c02>

<c02><did><container type="sfcaudioopenreel">FT-20027/16006</container><unittitle>Jarrell and Cockerham #3, Lowgap, N.C., 8 July 1971</unittitle><physdesc><genreform>1/4" Open Reel Audio</genreform></physdesc></did><scopecontent><p>Audio recording featuring Tommy Jarrell and Fred Cockerham; Recorded by Blanton Owen at the former home of Fred Cockerham in Lowgap, N.C.</p></scopecontent></c02>
```

Once your spreadsheet is complete, you can copy and paste the necessary lines or cells into the collection's XML finding aid.

Below are further suggestions on how to code an AV items at a minimum and moderate level. 

### Minimum (required):

```
<did> 

<container type="container type">AV item call number</container> 

<unittitle>Title</unittitle> 

<physdesc> 

<genreform>Format</genreform> 

</physfacet> 

</did> 
```

### Moderate:

```
<did> 

<container type="container type">AV item call number</container> 

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

<container type="sfcaudioopenreel">Audio item call number</container> 

<unittitle>Title, Place, Date: tape number</unittitle>     

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

##### Audio example:

```
<did> 

<container type="sfcaudioopenreel">FT-20009/1</container> 

<unittitle>Mike and Alice, Atlanta, Ga., 1977: tape 1 of 2</unittitle>     

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

<container type="videotape">Video item call number</container> 

<unittitle>Title, Place, Date: tape number</unittitle>   

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

##### Video example:

```
<did> 

<container type="videotape">VT-20009/1</container> 

<unittitle>Elizabeth Cotton, Chapel Hill, N.C., 1983: tape 1 of 2</unittitle>   

<physdesc> 

<genreform>Betacam SP</genreform> 

<extent>30 minutes</extent> 

<physfacet>edited master ; color ; sound (mono)</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>An interview with Elizabeth Cotton conducted by Mike Seeger.</p> 

</scopecontent> 

<processinfo><p>Processing information: Memo found with original container resides in Folder 3</p></processinfo> 
```

#### Film

```
<did> 

<container type="film">Film item call number</container> 

<unittitle>Title, Place, Date: tape number</unittitle> 

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

##### Film example:

```
<did> 

<container type="film">F-20009/1</container> 

<unittitle>Alice and Hazel, Chapel Hill, N.C., 1973: reel 1 of 2</unittitle> 

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

<extref href="[insert cdr link]"Digtial folder number</extref></container> 

<unittitle>Title, Place, Date</unittitle> 

<physdesc> 

<extent>Number of files</extent> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - source media, date of original files, note regarding access copies, etc</p></processinfo> 
```

##### Born-Digital example:

```
<did> 

<container type="digfolder"><extref href="https://cdr.lib.unc.edu/list/uuid:b699afe5-17e3-4020-a55b-a4746c0353f7">DF-20469/1</container> 

<unittitle>Fiddler's Grove Bluegrass Festival, 1973</unittitle> 

<physdesc> 

<extent>1 digital file</extent> 

</physdesc></did> 

<scopecontent> 

<p>An edited digital version of Brian Burch's Super 8mm footage (F-20469/1-9) set to traditional music. Edited by Brian and Gillen Burch.</p> 

</scopecontent> 

<processinfo><p>Processing information: The digital files were extracted from DVD. Original DVD files are dated 6 July 2005. An access .mp4 file was made from the DVD files for viewing purposes.</p></processinfo> 
```

#### AV Box:

As mentioned in the [Processing Levels](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#processing-levels) section, sometimes you may need to describe AV items at the box level. 


```
<did> 

<container type="avbox">AV box number</container> 

<unittitle>Title, Place, Date</unittitle> 

</did> 
<scopecontent><p>Brief description of contents.</p></scopecontent>

```


Below are examples of AV Box description, including a single box and range of boxes:

```
<did> 

<container type="avbox">1</container> 

<unittitle>Documentary project, 1980</unittitle> 

</did> 
<scopecontent><p>AV items related to a documentary film project produced in 1980 by Tom Davenport.</p></scopecontent>

```

```
<did> 

<container type="avbox">1-7</container> 

<unittitle>Apollo Records Test Pressings</unittitle> 

</did> 
<scopecontent><p>LP Test pressings arranged roughly alphabetically by artist.</p></scopecontent>

```

## Formats/Container types

The following section includes information on AV formats in Jitterbug metadata and finding aid description. 

### Audiovisual Box

When materials are being described at the box-level in finding aids, use the Audiovisual Box container type below. 

| **Finding Aid Display Name**                              | `<container type=>`     | Individual Item/Folder/Box Style        |
| ---------------------------------------------- | ------------------------| ------------------------------------- | 
| **Audiovisual Box**                               | avbox                      | box#                                 |

For intensive item-level description related to Jitterbug data entry and finding aid description, proceed to the Audio, Video, and Film sections below. These sections include information on:

- **Jitterbug Format**: format display name in [Jitterbug](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#jitterbug)   
- **Jitterbug Format ID**: unique ID given to each Jitterbug AV format type that is used primarily during [CSV import](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#csv-import)
- **SFC Item**: call number pre-fix assigned to AV items in the Southern Folklife Collection
- **SHC/UARMS/etc Item**: call number pre-fix assigned to AV items in the Southern Historical Collection, University Archives, North Carolina Collection, and Rare Book collecting units
- **Finding Aid `<container type=>`**: Finding Aid container types for the _type_ attribute in the [XML/EAD](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#xmlead) `<container>` tag. EAD container types across all formats can be found in Technical Services' [EAD] page(https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/EAD.md). 
- **Finding Aid Display Name**: AV format name displayed in finding aids
- **Finding Aid `<genreform=>` text**: Format name listed in the `<genreform=>` tag found in the [XML/EAD](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Audiovisual%20Materials.md#xmlead) `<physdesc>` tag. This metadata is usually more descriptive than the Finding Aid Display Name.

If you need assistance identifying AV formats, consult the Audiovisual Archivist or a Technical Services Processing Archivist. A great online resource for identifying AV is the Preservation Self-Assessment Program's Collection ID Guide: 

https://psap.library.illinois.edu/collection-id-guide 

EAD container types across all formats can be found in Technical Services' [EAD] page(https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/EAD.md).


### Audio

| **Jitterbug Format**             | Jitterbug Format ID     | SFC Item        |  SHC/UARMS/etc Item | Finding Aid `<container type=>`                   | Finding Aid Display Name                 | Finding Aid `<genreform=>` text |
| ---------------| ------------| --------------------- | --------------------- | --------------------- | --------------------- | --------------------- | 
| Audiocassette  | 28          | FS      | C    | sfcaudiocassette [FS]; audiocassette [C] | SFC Audio Cassette [FS]; Audiocassette [C] | Audiocassette |                
| Microcassette                  | 29                  | FS                     | C                              | sfcaudiocassette [FS]; audiocassette [C] | SFC Audio Cassette [FS-]; Audiocassette [C-] | Microcassette |                                     |
| 8-Track Tape                   | 30                  | 8T                     | 8T                              | 8T                                      | 8-Track Tape | 8-Track Tape                                     |                                   
| 1/4" Open Reel Audio           | 31                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     |1/4" open reel audio                             |
| 1/2" Open Reel Audio           | 32                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | 1/2" open reel audio                             |
| 1" Open Reel Audio             | 33                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | 1" open reel audio                               |
| 2" Open Reel Audio             | 34                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | 2" open reel audio                               |
| ADAT                           | 35                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | Alesis Digital Audio Tape (ADAT)                 |
| Digital Audio Tape (DAT)       | 36                  | DAT                    | DAT                            | dat                                     | Digital Audiotape     | Digital Audio Tape (DAT)                         |
| Hi8 (Audio Tape)               | 37                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | Hi8 [Audio]                                      |
| Data8                          | 38                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | Data8                                            |
| U-Matic (Audio Tape)           | 39                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | U-Matic [Audio]                                  |
| Beta (PCM-F1)                  | 40                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | Beta (PCM-F1) [Audio]                            |
| VHS (PCM-F1)                   | 41                  | FT                     | T                              | sfcaudioopenreel [FT]; audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | VHS (PCM-F1) [Audio]                             |
| Instantaneous Disc             | 45                  | FD                     | FD (legacy: D)                          | fd                                      | Instantaneous Disc     | Acetate disc / Lacquer disc / Instantaneous disc |
| Transcription Disc             | 46                  | TR                     | TR (legacy: D)                          | trans                                   | Transcription disc  | Transcription Disc             |                             |
| Wire Recording                 | 47                  | WR                     | WR                             | wr                                      | Wire recording                                   | Wire recording                                   |
| 45                             | 48                  | 45rpm                     | 45rpm (legacy: D)                           | 45                               | 45-rpm Disc | 45-rpm record                                    |
| 78                             | 49                  | 78rpm                     | 78rpm (legacy: D)                           | 78                               |  78-rpm Disc | 78-rpm record                                    |
| Cylinder                       | 50                  | CY                     | CY                             | cylinder                                       | Cylinder                                         | Cylinder                                         |
| MiniDisc                       | 51                  | MD                     | MD                             | md                                      | Mini-Disc | MiniDisc                                         |
| LP                             | 52                  | FC                     | FC (legacy: D)                          | audiodisc                               | Audiodisc | LP record                                        |
| Flexi Disc                     | 53                  | FC                     | FC (legacy: D)                        | audiodisc                               | Audiodisc | Flexi disc                                       |
| Analog Disc                    | 54                  | D                      | D                        | audiodisc                               | Audiodisc | Metal stamper                                    |
| NAB Catridge                   | 56                  | FT                     | T                              | sfcaudioopenreel [FT] audiotape [T]     | SFC Audio Open Reel [FT]; Audiotape [T]     | NAB cartridge                                    |

### Video

| **Jitterbug Format**             | Jitterbug Format ID     | SFC Item        |  SHC/UARMS/etc Item | Finding Aid `<container type=>`                   | Finding Aid Display Name                 | Finding Aid `<genreform=>` text |
| ---------------| ------------| --------------------- | --------------------- | --------------------- | --------------------- | --------------------- | 
| Betacam  | 7          | VT      | VT    | videotape | Videotape | Betacam    |     
| Betacam SP                     | 8                   | VT                     | VT                             | videotape | Videotape             | Betacam SP                     |
| Betamax                        | 9                   | VT                     | VT                             | videotape | Videotape             | Betamax                        |
| U-Matic                        | 10                  | VT                     | VT                             | videotape | Videotape             | U-Matic                        |
| U-Matic SP                     | 11                  | VT                     | VT                             | videotape | Videotape             | U-Matic SP                     |
| VHS                            | 12                  | VT                     | VT                             | videotape | Videotape             | VHS / VHS-C / S-VHS            |
| HDCAM                          | 13                  | VT                     | VT                             | videotape | Videotape             | HDCAM                          |
| DVCAM                          | 14                  | VT                     | VT                             | videotape | Videotape             | DVCAM                          |
| MiniDV                         | 15                  | VT                     | VT                             | videotape | Videotape             | MiniDV                         |
| Digital Betacam                | 16                  | VT                     | VT                             | videotape| Videotape             | Digital Betacam                |
| Hi8                            | 17                  | VT                     | VT                             | videotape| Videotape             | Hi-8                           |
| Video8                         | 18                  | VT                     | VT                             | videotape| Videotape             | Video8                         |
| Digital 8                      | 19                  | VT                     | VT                             | videotape| Videotape             | Digital 8                      |
| D-2                            | 20                  | VT                     | VT                             | videotape| Videotape             | D-2                            |
| M-Format                       | 21                  | VT                     | VT                             | videotape| Videotape             | M-Format                       |
| 2" Open Reel Video             | 22                  | VT                     | VT                             | videotape| Videotape             | 2" open reel video             |
| 1" Open Reel Video             | 23                  | VT                     | VT                             | videotape| Videotape             | 1" open reel video             |
| 1/2" Open Reel Video           | 24                  | VT                     | VT                             | videotape| Videotape             | 1/2" open reel video           |

It's worth noting that there are also a handful of legacy SFC Call number prefixes for video formats that are no longer in use, including **VOR** (video open reel), **VUT** (video U-Matic), **VBC** (video Betacam) and **VHS** (VHS). You may run accross these pre-fixes when working with legacy collections, such as Southern Folklife Collection Moving Image Materials #30002. 

### Film

| **Jitterbug Format**             | Jitterbug Format ID     | SFC Item        |  SHC/UARMS/etc Item | Finding Aid `<container type=>`                   | Finding Aid Display Name                 | Finding Aid `<genreform=>` text |
| ---------------| ------------| --------------------- | --------------------- | --------------------- | --------------------- | --------------------- | 
| 35mm                           | 1                   | F                      | F                              | film | Film                  | 35mm motion picture film       | 
| 16mm                           | 2                   | F                      | F                              | film | Film                  | 16mm motion picture film       |
| Super 8mm                      | 3                   | F                      | F                              | film | Film                  | Super 8mm motion picture film  |
| 8mm                            | 4                   | F                      | F                              | film | Film                  | 8mm motion picture film        |
| 9.5mm                          | 5                   | F                      | F                              | film | Film                  | 9.5mm motion picture film      |
| Filmstrip                      | 6                   | F                      | F                              | film | Film                  | Filmstrip                      |
| Film preservation instance     | TBD                   | FPI                    | FPI                              | fpi | Film                   | 16mm motion picture film preservation instance         | 



## Subject headings

A great resource for folklore sound recording collections is the **American Folklore Society's Ethnographic Thesaurus:** http://id.loc.gov/vocabulary/ethnographicTerms.html 

Listed below is a local controlled vocabulary for music-based and/or AV centric collections. Subject headings are arranged loosely by genre or subject. For more widely applicable subject terms (i.e.: Folk music., Folk songs., Dance music., etc), it may be useful to further specify the heading with a geographic location (i.e. Folk music--North Carolina.).  

#### Blues and R&B:

- Blues (Music)
- Blues musicians.
- Doo-wop (Music)
- Harmonica music.
- Piedmont blues.
- Popular music--United States.
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

# Labeling and putting stuff away

This section discusses rehousing, labeling, box types, and shelving locations of AV items. Plan to cross-reference this section with Technical Services general documentation on [Labelling and Putting Stuff Away](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Labelling%20and%20Putting%20Stuff%20Away.md), which includes crucial information on recording locations in ArchivesSpace.

## Rehousing Materials

Apart from moving image film, it is preferable to leave AV materials in their original containers since these containers often contain information about the original stock, as well as container notes created by the creator or donor of the collection. Exceptions to this include original containers with severe preservation or conservation concerns, such as mold or an inability to properly contain the item at hand.  

Whenever an AV material is rehoused, transcribe all titles and container notes from the original container into the item's Jitterbug "Container note" field and photocopy or digitally photograph the original container. Place the photocopy or photograph in the collection’s control file or the curatorial unit's Department Drive until proper procedures for documenting original containers are developed.  

Unlike audio and video formats, moving image film is ideally hand inspected, placed onto archival cores, and rehoused into archival cans. Technical Services decided how to provide housing for film on case-by-case basis. Consult the Audiovisual Archivist about film inspection and rehousing before proceeding with moving image materials.  

## AV item labels

Once you have retrieved the correct AV item call numbers from Jitterbug (either via the Jitterbug interface or via Jitterbug [data export](#data-export)), see “How to Create Item level AV Labels” document, which covers how to create AV item labels using Microsoft Word's mail merge: G:\wilson\ts\archival\labels\AV labels\How to Create Item AV Labels.docx

There are two label templates for AV item labels - front facing foil-backed labels and spine foil-backed labels. Blank pages of both label types are located in Technical Services' main processing room.

**Templates for both label types can be found in the Departments drive:**  
G:\wilson\ts\archival\labels\AV labels\AV_front_labels  
G:\wilson\ts\archival\labels\AV labels\AV_spine_labels

Use whichever label and placement makes sense for the material- generally speaking, processing archivists use front facing labels for circular items, like audiodisc formats and open reel open reel audiotapes, and use spine labels for more cartridge based materials, like audiocassettes, digital audiotapes (DAT), and videotapes. No matter which label you choose, be sure to place it on the AV item's box or case, rather than on the physical media.  

Moving image films are a bit of an outlier when it comes to labels. If possible, use the Brother P-touch label maker located on level 10 to create a call number label (size 36 font) and adhere label to the side of film can. Hand write the title in all caps to the right of the call number label.       
 
Sample images of formats and label placement below:    
 
![open reel audiotape with front facing label](https://github.com/annewell/images/blob/main/Processing_OpenReelLabelssmall.png)    
_Front facing label on an open reel audiotape box_

![audiocassettes with spine labels](https://github.com/annewell/images/blob/main/Processing_CassetteLabels.png)    
_Spine label on audiocassette cases_

![audiocassettes with spine labels](https://github.com/annewell/images/blob/main/Processing_VideoLabels.png)    
_Spine label on videotape cases_
  
![a stack of motion picture film cans with labels written on each can](https://github.com/annewell/images/blob/main/Processing_FilmLabelsmall.png)  
_Labels on motion picture film can_

### Exceptions to the rule

Do not place labels on the spine when pertinent information or existing labels are found externally on the container’s spine or if the label does not properly fit on the spine. If either of these instances occur, place label on the top left front of the item. Sample image below:

![audiocassette with front facing label](https://github.com/annewell/images/blob/main/Processing_CassetteLabels2.png)  
_Front facing label on audiocassette_

Consult SFC staff when there are questions of preservation when labeling items. For extremely rare or unique items, it is possible to place a label on a custom-made Mylar sleeve that is placed over the item. Sample image below: 

![LP with mylar sleeve that lists call number](https://github.com/annewell/images/blob/main/Processing_LPSleeveLabel.png)  
_LP with front facing label placed on custom-made Mylar sleeve_

## AV box types and labels

### AV box types

Small to medium-sized AV materials require additional housing into archival boxes, while larger formats do not require additional housing.

#### AV items that do not require boxing:

**Audio:**

    - ¼” Open Reel Audio 
    - ½” Open Reel Audio 
    - 1” Open Reel Audio 
    - 2” Open Reel Audio 
    - Videotape formats used as audio, such as ADAT and VHS (PCM-F1)

**Motion Picture Film:**

    - 35mm 
    - 16mm 
    - Super 8mm 
    - 8mm 
    - 9.5mm
    - Filmstrips

**Open Reel Videotape:**

    - ½” Open Reel Video 
    - 1” Open Reel Video 
    - 2” Open Reel Video

Proceed to [Shelving](#shelving) if you have any of the materials listed above.  

#### AV items that require boxing

The small to medium-sized AV materials AV formats that do require additional housing into archival boxes are listed below with the appropriate box title and box type. 

Please note that there are three distinct boxing systems for AV items, including one for all collecting units besides the Southern Folklife Collection ("Wilson AV Box") and two distinct boxing systems for the Southern Folklife Collection ("SFC AV Box" and "Legacy SFC AV Box"). These three box systems are listed below with their associated formats and archival box type. (It can be tricky at first to get a hang of all of these different boxing systems - if you ever have a question, please feel free to consult the Audiovisual Archivist or a Technical Services processing archivist. We're here for you!)

**Wilson AV Box**  
Collecting units: Southern Historical Collection, University Archives, Rare Books Collection, North Carolina Collection

Use this boxing system for all collecting units besides the Southern Folklife Collection.

| Box Title                 | Format(s)                     | Box Type               |
| ------------------------- | ----------------------------- | ---------------------- |
| 8-Track Tapes             | 8-Track tape                  | Archival CD            |
| Audiocassettes            | Audiocassette; Microcassettes | Archival Audiocassette |
| Digital Audio Tapes (DAT) | DAT                           | Archival Audiocassette |
| MiniDiscs                 | MiniDisc                      | Archival Audiocassette |
| Audiodiscs (small)      | 45s, 7" LPs & Flexidiscs           | Archival 45     |
| Audiodiscs (medium)      | 10 and 12" LPs, 78s, and Instantaneous discs            | Archival LP (blue)     |
| Audiodiscs (large)      | Transcription Discs             | Archival Transcription Disc     |
| Videotape | Betacam; Betacam SP; Betamax; Digital Betacam; U-Matic; VHS; D-2; M-Format; VHS-C; HDCAM; DVCAM; MiniDV; Hi8; Video8; Digital 8 | Paige Box   

**SFC AV Box**  
Collecting unit: Southern Folklife Collection

Use this boxing system for SFC AV materials with "collection slash" call numbers, like "FS-20511/1" for example.

| Box Title                 | Format(s)                     | Box Type               |
| ------------------------- | ----------------------------- | ---------------------- |
| SFC 8-Track Tapes*             | 8-Track tape                  | Archival CD            |
| SFC Audiocassettes*            | Audiocassette; Microcassettes | Archival Audiocassette |
| SFC Digital Audio Tapes (DAT)* | DAT                           | Archival Audiocassette |
| SFC MiniDiscs*                 | MiniDisc                      | Archival Audiocassette |
| SFC Audiodisc       | Audiodisc stampers           | Archival LP (blue)     |
| SFC Transcription Discs*       | Transcription Discs           | Archival Transcription Disc     |
| SFC Instantaneous Discs*       | Instantaneous Discs           | Archival Instantaneous Disc (off-white)     |
| SFC LPs       | 7, 10, and 12" LPs, Flexidiscs           | Archival LP (blue)    |
| SFC 45s       | 45s           | Archival 45     |
| SFC 78s       | 78s           | Archival 78     |
| SFC Videotape | Betacam; Betacam SP; Betamax; Digital Betacam; U-Matic; VHS; D-2; M-Format; VHS-C; HDCAM; DVCAM; MiniDV; Hi8; Video8; Digital 8 | Paige Box   

**Legacy SFC AV Box**  
Collecting unit: Southern Folklife Collection

Use this boxing system for legacy SFC materials with consecutive call numbers that span SFC collections (FS-16012, FS-16013, FS-16014, and so on, for example). AV items with legacy style call numbers have separate boxes and label types, and are shelved in a separate location. More on that below under [AV box labels](#av-box-labels) and [Shelving](#shelving).

| Box Title                 | Format(s)                     | Box Type               |
| ------------------------- | ----------------------------- | ---------------------- |
| SFC 8-Track Tapes             | 8-Track tape                  | Archival CD            |
| SFC Audiocassettes            | Audiocassette; Microcassettes | Archival Audiocassette |
| SFC Digital Audiotapes (DAT) | DAT                           | Archival Audiocassette |
| SFC MiniDiscs                 | MiniDisc                      | Archival Audiocassette |
| SFC Transcription Discs       | Transcription Discs           | Archival Transcription Disc     |
| SFC Instantaneous Discs       | Instantaneous Discs           | Archival Instantaneous Disc (off-white)     |

Before you begin boxing and shelving AV materials, check on level 10 to see if there is space in the last box located in the box title sequence - a flag stating "space available" should be visible. If there is indeed room in the last box of a sequence, box as many items that will fit before creating new AV boxes and box labels.

When boxing, try to organize items by call number in the box. Place items in a top-down order starting on the top left of the box. Be consistent as to how you place items in the box(es). Place call numbers facing out when possible. Try not to place items on top of each other. There are no strict rules for boxing materials - use your best judgement. The goal is easy access for patron requests and digitization. Annotated (and perhaps overkill) examples below: 

**Ideal arrangement of audiocassettes in archival audiocassette box:**   
![cassettes arranged in audiocassette box with arrows illustrating ideal box arrangement](https://github.com/annewell/images/blob/main/Shelving_BoxArrangement1.png)

**Ideal arrangment of DATS in archival audiocassette box:**  
![DATS arranged in audiocassette box with arrows illustrating ideal box arrangement](https://github.com/annewell/images/blob/main/Shelving_BoxArrangement2.png)

**Ideal arrangement of videotapes in paige box:**  
![videotapes arranged in paige box](https://github.com/annewell/images/blob/main/Shelving_VideoBoxArrangement.png)

### AV box labels

Label templates for each shared box title resides in the Departments drive: G:\wilson\ts\archival\labels\AV labels

These templates include labels for all 3 box types mentioned above, including both Southern Folklife Collection label types. Templates are arranged by collecting unit: "SFC" and "non SFC".

![box labels in folders on metal shelving](https://github.com/annewell/images/blob/main/Shelving_BoxLabelsresize.jpeg)

Please note that existing labels for select shared AV boxes, such as "Videotape box", "Audiocassette box", etc, are stored in file folders located in Technical Services' sweatbox space (that transitional space between the main processing room and the stacks), illustrated above. Create and print additional box title labels as needed.

### Images of box types and labels

Below are images of select AV boxes for all three AV boxing methods (Wilson AV box, SFC AV box, and legacy SFC box) for reference.

**Wilson AV box titles and types:**

![videotape box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_Videotapebox.JPEG)  
_Videotape box title on paige box with "space available" flag in the most recent box._

![Audiocassettes stored on metal shelving](https://github.com/annewell/images/blob/main/Shelving_Audiocassettes.JPEG)  
_Audiocassettes box title on archival audiocassette box type. Note the "space available" flag in the most recent box._

![small audiodisc box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_AudiodiscsSmall.jpeg)  
_Audiodiscs (small) box title on archival 45 box type._

![medium audiodisc box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_AudiodiscsMedium.JPEG)  
_Audiodiscs (medium) box title on archival LP disc box type._

![large audiodisc box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_AudiodiscsLarge.JPEG)  
_Audiodiscs (large) box title on archival transcription discs box type._

**Southern Folklife Collection AV box titles and types below:**

![Southern Folklife videotape box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCVideotape.JPEG)  
_SFC videotape box title on paige box._

![Southern Folklife Colleciton audiocassette box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCAudiocassetteBox.JPEG)    
_SFC audiocassettes box title on archival audiocassette box.._

![Southern Folklife Colleciton Instantaneous Discs box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCInstantaneousDiscs.JPEG)  
_SFC Instantaneous Discs box title on archival instantaneous disc box type._

![Southern Folklife Colleciton Instantaneous Discs box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCTranscriptionDiscs.JPEG)    
_SFC Transcription Discs box title on archival transcription discs box type._

![Southern Folklife Colleciton LP box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCLPs.JPEG)  
_SFC LP box title on archival LP box type._

![Southern Folklife Colleciton 8-track box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFC8track.jpeg)  
_SFC 8-track box title on archival CD box type._


**Legacy Southern Folklife Collection AV box titles and types below:**

![Southern Folklife Colleciton legacy audiocassette box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCLegacyAudiocassetteBox.JPEG)    
_Legacy SFC audiocassettes box title on archival audiocassette box type, with handwritten call numbers._

![Southern Folklife Colleciton Instantaneous Discs box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCInstantaneousDiscsLegacy.JPEG)  
_Legacy SFC Instantaneous Discs box title on archival instantaneous disc box type, with handwritten call numbers._

![Southern Folklife Colleciton Instantaneous Discs box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_LegacySFCTranscriptionDiscs.JPEG)    
_Legacy SFC Transcription Discs box title on archival transcription discs box type._

![Southern Folklife Colleciton 8-track box on metal shelving](https://github.com/annewell/images/blob/main/Shelving_SFCLegacy8track.jpeg)  
_Legacy SFC 8-track box title on archival CD box type._

## Shelving

AV items are stored by format on level 10 in the 1952, or "orange", section of Wilson Library's closed stacks (except for several hundred motion picture films stored remotely at the Library Service Center (LSC), but let's not get into that now). Select AV formats, like open reel audio and moving image film, are also shelved by collecting unit.

As previously noted, Southern Folklife Collection AV items are shelved separately from other collecting units at Wilson. SFC also has two distinct call number systems for select formats that are shelved independently from one another. 

Below are the current shelving locations for AV items arranged by format, collecting unit, and SFC call number type (when appropriate).

### Open reel audio

Includes 1/4" Open Reel Audio, 1/2" Open Reel Audio, 1" Open Reel Audio, 2" Open Reel Audio, ADAT, Hi8 (Audio Tape), Data8, U-Matic (Audio Tape), Beta (PCM-F1), VHS (PCM-F1), NAB Cartridge. Shelve as-is. Does not require boxing. 

    SFC (FT-100 through FT-18000s): N.5 a through N.3 a (currently: N.3 a.66) 
    
    SFC (“FT-_ _ _ _ _/_”): K.18 b through K.20 b (currently: K.20 b.8) 

    SHC (“T”): K.27 a through K.27 b (currently: K.27 b.14) 

    UARMS (“T”): N.2 a through N.1 b (currently: N.1 b.13) 

### Audiocassette

Includes audiocassettes and microcassettes. Formats require box storage. 

    SFC (FS-100 through FS-18000s): K.24 a through K.23 b (currently: K.23 b.6) 

    SFC (“FS-_ _ _ _ _/_): K.23 b (currently: K.23 b.46) 

    SHC/UARMS/RBC (“C”): K.26 b (currently: K.26 b.27) 

### Audiodiscs

Includes Instantaneous disc, Transcription discs, 45s, 78s, LP, Flexi disc, Analog discs. Formats require box storage. 

    SFC Instantaneous discs (“FD-“): K.3 b (currently K.3 b.14) 

    SFC Transcription discs (“TR-“): K.3 b through K.4 a [bottom row] (currently: K.4 a.30) 

    SFC 45 (“45-“): K.3 b (currently: K.3 b.11) 

    SFC 78 (“78-“): K.3 b (currently: K.3 b.11) 

    SFC LP and Flexi disc (“FC-“): K.3 b (currently: K.3 b.12) 

    SFC Analog disc (“D-“): K.3 b (currently: K.3 b.12) 

    SHC/UARMS/RBC small audiodiscs (45s, Flexi discs, small-sized Instantaneous discs): N.1 b (currently: N.1 b.42) 

    SHC/UARMS/RBC medium audiodiscs (LPs, 78s, medium-sized Instantaneous discs): N.1 b (currently: N.1 b.51) 

    SHC/UARMS/RBC large audiodiscs (Transcription discs, large-sized Instantaneous discs): N.1 b [bottom row] (currently: N.a b.63) 

### Digital Audio Tape (DAT)

Includes Digital Audio Tapes (DATs) 

    SFC (DAT-100s through DAT-600s): KK.11 a. 1 (currently: KK.11 a. 1) 

    SFC (“DAT-_ _ _ _ _/_“): KK.11 a through KK.12 a (currently: KK.12 a. 3) 

    SHC/UARMS/RBC (“DAT-“): N.1 b (currently: N.1 b.57) 

### MiniDisc 

Includes MiniDisc 

    SFC (MD-100s): KK13 a (currently: KK13 a.1) 

    SFC (“MD-_ _ _ _ _/_“): KK13 a (currently: KK13 a.1) 

    SHC/UARMS/RBC (“MD-“): TBD! 

### 8-Track Tape 

Includes 8-track tapes 

    SFC (“8T”): K.3 b (currently K.3 b.21) 
    
    SHC/UARMS/RBC (“8T”): TBD!

### Cylinder

Includes cylinders 

    SFC/SHC/UARMS/RBC (“CY”): K.3 b (currently: K.3 b.32) 

### Wire Recording

Includes wire recordings 

    SFC/SHC/UARMS/RBC (“WR-“): K.3 b (currently K.3 b.22) 

### Videotape (boxable videotapes)

Includes Betacam, Betacam SP, Betamax, Digital Betacam, U-Matic, VHS, HDCAM, DVCAM, MiniDV, Hi*, Video8, Digital 8, D-2, M-Format 

    SFC (“VT-“): M.2 a; M.2 b; K.1 b; K.2 a (currently: K.2 a.27) 

    SHC/UARMS/RBC (“VT-“): K.5 b through K.9 b (currently: K.9 b.26) 

### Videotape (large open reel)

Includes 2" Open Reel Video, 1" Open Reel Video, 1/2" Open Reel Video 

    SFC (“VT-“): K.2 a [bottom row] (currently: K.2 a.36) 

    SHC/UARMS/RBC (“VT-“): K.5 a through K.5 b [bottom row] (currently: K.5 b.47) 

### Film

Includes 35mm, 16mm, Super 8mm, 8mm, 9.5mm motion picture film and Filmstrips 

    SFC (“F-“): K.10 a through K.11 a (currently: K.11 a.10) 

    SHC (“F-“): K.8 b through K.11 a (currently: K.11 a.10) 

    UARMS (“F-“): K.10 b through K.11 a (currently: K.11 a.10) 
    
Full-coat magnetic soundtracks

    SFC, SHC, UARMS (“F-“): KK. 15 a (currently: KK.15 a.2)
    
## Creating locations in ArchivesSpace

Once AV items are shelved in their appropriate location, record the location in ArchivesSpace. Visit Technical Services' [Labelling and Putting Stuff Away](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/main/Labelling%20and%20Putting%20Stuff%20Away.md#creating-locations-in-archivesspace) for helpful instructions on how to record AV item locations in ASpace.

An important distinction to note is that you can add AV locations either in a Resource record or an Accession record in ArchivesSpace. Add locations to the Resource record when AV items are described or listed out in the collection finding aid (or are planning to be described by Technical Services). When AV materials are not described in a collection finding aid, such as a collection-level finding aid, add AV item locations to the appropriate Accession record.

# Resources  

This documentation page is not the result of a single individual! As the Audiovisual Archivist at Wilson Library, I lean on my Wilson Library colleagues (endless thanks to them!) and acknowledge the many smart & thoughtful people in the larger archives field who have presented and published widely about processing archival AV materials. Below is a growing & ever-evolving list of some recommended resources to check out if you haven't already. Solidarity to the AV people out there - wishing you all the best (& permanent funding for all your endeavors).:

- University of Illinois at Urbana-Champaign's [Preservation Self-Assessment Program: "Collection ID Guide: Audiovisual Materials"](https://psap.library.illinois.edu/collection-id-guide#audiovisual)

a great resource (with lots of photographs) for identifying analog audiovisual formats. 

- Megan McShea, Smithsonian Archives of American Art, ["Guidelines for processing archival collections with audiovisual material"](https://www.aaa.si.edu/tags/documentation)

a thorough and thoughtful approach to processing archival audiovisual materials in a finding aid context.

- New York University Libraries, ["Descriptive Policies on Audiovisual and Born-digital Materials"](https://docs.google.com/document/d/1Zcvp57201jEgsGZgT8Up1c7nIWAwdtHHBMZn3NYogRs/edit)

a peek at another academic instutition's documentation on descriptive policies for audiovisual and born-digital materials (thank you NYU folks!).

- [Association of Moving Image Archivists (AMIA)](https://amianet.org/); [Association for Recorded Sound Collections (ARSC)](http://www.arsc-audio.org/index.php); [International Association of Sound and Audiovisual Archives (IASA)](https://www.iasa-web.org/); [International Federation of Film Archives (FIAF)](https://www.fiafnet.org/)

professional organizations dedicated to the preservation and access to our collective AV heritage.

- mentors past and present! Andy Uhrich, Michelle Puetz, Nancy Watrous, Carolyn Faber, Andrew Lampert, Rick Prelinger, and so many more <3

# Endnotes

^1 item-level streaming access restrictions ("Open", "Campus", or "Closed") are determined by the curatorial unit. Access restrictions are ideally determined during intake or acquisition. Processing Archivists may need to correspond with the curatorial unit to gather additional item-level restrictions.  


