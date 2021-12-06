Updated July 2020 by Jodi Berkowitz.

# Overview

- [Creating new MARC records](#creating-new-marc-records)
- [Editing existing MARC records](#editing-existing-marc-records)
- [Headings for archival records (authority work)](#headings-for-archival-records-authority-work)

***

# Creating new MARC records

## Create a new record

1. Select collection for which you will create a record
   - File > Local File Manager > xx.bib.db
   - Double click, close
2. New mixed material catalog record: Ctrl-Shift-I
3. Bring up constant data (template): Ctrl-B
   
   OR
   
4. Identify record to use to derive new record
   - F3 brings up save file
   - Choose record, copy OCLC number
   - Paste OCLC number into search box (# first)
5. Edit > Derive > New master record (Ctrl-Alt-C)
   - Yes to transfer fixed field values
   
## Completing the fields

If using constant data, most of the fixed fields should be set and the fields that need completing should be clear (Ctrl-Shift-I, Ctrl-B, enter name of constant data template) 

Fixed fields mostly remain the same

### Fixed Fields

**Date(s)**

Select type of date (i: inclusive; s: single); enter dates 

**Country/location)**
  
 Enter country/location (xxu: US; ncu: NC)
 
 ### 040
 
 enter ‡b eng and ‡e dacs **(Ctrl-D to insert ‡)**

### 041 : non-English language

If materials in a language other than English are present:

  enter ‡a lang code, repeat ‡a as needed
  
### 100 : Creator

Copy and paste from finding aid
 
  - Right click > Control single heading (F11)
  - ‡d for dates, ‡c for qualifier
  - Person: 100 1 _ 
  - Family: 100 3 _
  - Corporate body: 110 1 _
  - See Michelle's documentation (below) for forming family and other headings
  
### 245 1 0 : Title

Copy and paste from finding aid

  - If no creator, 245 0 0 (no other changes)
  - Collection in lowercase
  - ‡f for dates, ‡g for bulk dates
  - NO period at end of dates
  
### 300 _ _ : Extent

**"approximately XXX ‡f items ‡a (xx ‡f linear feet)** (no period at end)

  - Remove, edit as needed depending on collection

### 500 _ _ : Citation note

**"In the xxx, University of North Carolina at Chapel Hill (#)"**

  - Possibly other notes, depending
  
### 520 8 _ : Abstract

Copy and paste abstract from finding aid (no period at end)
Biographical information goes here as well (545 no longer used)

### 506 1 _ : Access restrict

  - Flashers have a more detailed note here, but no other special treatment (no period at end)
  - If no restriction, use **506 0 _ No restrictions**
  
### 530 _ _ : Additional form of material

No period at end

### 540 _ _ : Use restrict

No period at end

### 541 _ _ : Source of Acquisition

**"Acquired ‡d date"** (no period at end)

### 544 1 _ : Related materials

**"See also ‡d collection name (#) in the ‡a collection, University of North Carolina at Chapel Hill"**

### 546 _ _ : Language note

**"English"** (no period at end)

### 600/610/650/651 : Subject access fields

  - Copy and paste subject headings from finding aid
  - Subfield codes
    - ‡d dates
    - ‡v form
    - ‡x general
    - ‡y chronological
    - ‡z geographic
  - Clean up mess
  - Control headings 
    - Shift + F11 for all
    
### 856 4 2 : Electronic Location and Access  

**"‡3 Finding aid ‡u URL"**

## Finishing up

1. Click on the R in the menu bar

2. Click on the green check next to the R

   - Make any corrections as instructed, if needed
   
3. Click on the yellow up arrow button, two down from R

   - This creates the OCLC#, note it on the blue sheet

4. Run marcro: Ctrl-J
 
   - this adds 099, 049, 949
   - For a new collection:
     - Choose title not in Millennium
     - Copy and notes
     - Have 099 local call #
     - ‡a collection # (include leading zero for SHC collection)
   - For a collection with a collection-level record in Sierra:
     - Choose title in Millennium
     - Copy and notes
     - Have 099 local call #
     - ‡a collection # (including leading zero for SHC collection)
     
5. Bring to Sierra

   - Export using green arrow button (F5)
   - Open Sierra, search by title or local call number
   - Hit summary, confirm item record is there
   - Add STATS note- "Cataloged FY 2020-21" using "j" or macro if set up (e.g. F7)
   - For a collection with a collection-level record in Sierra, edit status in item record and edit initials and cat date
   - Save
   - Close pop up window in Connexion
   
6. Enter in stat sheet

7. Hit F4 to save to local save file

8. Enter OCLC # in Proc Rec

   - TS > archival > processing database > processing_database.db


# Editing existing MARC records

### 1. In Sierra, search for the collection whose record you want to edit
     
  - Copy the OCLC record number from the **001** field
  - Close the record (you cannot overlay a new record onto an open record)
      
### 2. In Connexion, open the record you want to edit (search: #OCLCnumber)

### 3. Make necessary updates according to the blue sheet

   - Note that dates need to be updated in two locations:
      - Fixed fields
      - Collection number
   - Ctrl-D for subfield
      
### 4. Other things to check for:

   - Add ‡e dacs in the **040**, if it isn't there already
   - Remove **545**, update **520**
   - **546 _ _** English
   - **506 0 _** No restrictions (if there's not already a **506** listing in the restrictions)
   - **856 4 2** the finding aid URL is current
   
### 5. After making the desired edits

  - Click on R
  - Click on the check mark
  - Control headings if needed (Shift + F11)
  - Action > Replace record (Alt + F10)
  
### 6. Bring the record to Sierra

  - Export (F5)
  - Open the record in Sierra
      - When you export the record, it will automatically put the cat date as the current date. Then you have to change it back to what it was (if you're not sure, you can use the "created" date that appears at the top of the record) and add a 599 field with LTIEX
    - Add 599 LTIEXP if 1xx, 240, 4xx, 6xx, 7xx, 8xx edited (NOT 2xx, 3xx, 5xx)
  - Open the summary
    - Update the cat date in the internal note (“lls cat date 16 Feb, 2018”) - "x" for internal note
    - If there are older codes from a previous ILS, they can be deleted (the bottom of the summary should only include the collection call number and the cat date info) 
    - Save 
    
### 7. Enter in stat sheet under OCLC enhance and Millennium edits sections

### 8. Save to local file (F4)


# Headings for archival records (authority work)

## Contents

- Family names as creators
- Authority records for family names
- Family names as subjects
- Searching for the authority file
- Personal name headings
- Subject headings

## Family names as creators

When used as creators, family names should have qualifiers added to differentiate them from other families of the same name. 

Some examples from the authority file: 

- Johnson (Family : ǂg Johnson, Benjamin F. (Benjamin Franklin), 1818-1905) 
- Johnson (Family : ǂd 1804-1962 : ǂc Me.) 
- Jones (Family : ǂd 1797- : ǂc South Carolina) 
- Smith (Family : ǂg Smith, Upton Treat, 1843-1925) 

**RDA 10.11** covers the rules for constructing family names.  You’ll always start with the name of the family, with (Family) in parentheses following the name, followed by any other qualifiers. 

The other qualifiers that can be used are as follows:

- Dates associated with the family, in **$d**
- Place associated with the family, in **$c** 
- Prominent member of the family, in **$g**.  The name should be given in inverted order, last name first, in the same form that the person is established in the authority file or given as a heading in your record, except that any MARC coding will be removed within the **$g**. 

Family names as creators will be coded **100 3_ or 700 3_** in the MARC record. 

## Authority records for family names

In the family name authority record: 

- 376 Families ǂ2 lcsh 
- 376 ǂb [name of progenitor, if in the 100] ǂ2 naf 
- 500 1_ ǂw r ǂi Progenitor: ǂa 
- 500 1_ ǂw r ǂi Family member: ǂa   

In related personal name authority records: 

- 500 3_ ǂw r ǂi Descendants: ǂa 
- 500 3_ ǂw r ǂi Family: ǂa 

## Family names as subjects

The types of heading described above for family names as creators are not eligible to be used as subjects.  Family names as subjects will just be in the form “Smith family” or “Jones family,” with no added qualifiers.  These should be coded as **600 34**: 

- 600 34 Cameron family. 
- 600 34 Battle family. 

Using second indicator **4** (source not specified) instead of second indicator **0** (Library of Congress subject headings) will prevent the authority vendor from flipping unauthorized family names to their authorized forms. 

## Searching the authority file

You can search the LC authority file for names and subjects at http://authorities.loc.gov/.  Choose Subject Authority Headings or Name Authority Headings, as appropriate.  Both personal and corporate names are searched under Name Authority Headings.  Subject Authority Headings is for topical headings. 

## Personal name headings

Say you want to find the authorized heading for the musician Paul Brown.  Search by last name, first name in the authority file and you get this (plus many more). 

![screenshot](https://user-images.githubusercontent.com/58087302/78273256-9a629300-74dc-11ea-82b3-2d78b355af8e.png "Brown personal name headings 1")

You may know that Paul Brown was born in 1952 and be able to jump down to this part of the list: 

![screenshot](https://user-images.githubusercontent.com/58087302/78273750-47d5a680-74dd-11ea-8bd7-ed61e3b9ae2d.png "Brown personal name heading 2")

Click on the red button to the left of each heading and you’ll eventually be taken to the authority record (for some reason this requires many more steps than it should), which should give you an idea of whether or not each person is likely to be the one you want.  Some authority records have a lot of information and some have very little.  The record for Brown, Paul, 1952- looks like this: 

![screenshot](https://user-images.githubusercontent.com/58087302/78273911-6fc50a00-74dd-11ea-9181-dc22688eea3f.png "Brown personal name heading 3")

So this looks likely to be the person represented in an SFC collection.  You’ll copy the form that appears in the 100 field and use that in your finding aid.  Any 400 fields are cross-references that are there to lead you to the 100 field.  500 fields are see also references that link two related entities that are both established (e.g., John Lennon and the Beatles). 

If you’re searching a common name and you don’t want to go through the whole list of records in the authority file, a shortcut can be to start in our local catalog.  If the person is a folk musician, you can search on their name and limit to SFC as a location and possibly find the correct heading that way.  But, remember!  Once you’ve found a heading, make sure you go back to the LC authorities site and pull up the authority record there to make sure the heading is for the right person.  We have plenty of incorrect name headings in our catalog that don’t match the authority file, so we can’t blindly follow what is in the UNC catalog and assume that it’s correct. 

So, what do you do if you can’t find an authority record for the person you’re looking for?  In that case, you can construct your own heading, but you have to make sure it is different from any established headings in the authority file, and that it’s consistent with headings used already in the UNC catalog.  If you don’t find anything in the authority file, you should search the UNC catalog (preferably the classic catalog, http://www2.lib.unc.edu/webcat/, which is better for doing this kind of search) to see if the person has appeared already in our catalog, and if so, copy the form found there. 

If there’s nothing in either the authority file or the UNC catalog, you can formulate a name heading—usually last name, first name, with birth and/or death dates if available.  

Examples:     

- Larman, Howard.
- Michal, William Norwood, Sr., 1906-1991.

If you don’t have any dates to use to differentiate someone with a common name, you can add a qualifier in parentheses.  

Examples: 

- Cohen, Mike (Guitarist)
- Adams, Nicholas (Photographer)

A note on the form of name headings—the authority file is wildly inconsistent in how people are established.  Some people get the full birth date, death date, middle name treatment (e.g., Ashe, Samuel A. (Samuel A'Court), 1840-1938) while others have very simple headings (e.g., Haggard, Merle).  As a general rule, birth and death dates are added if they’re readily available at the time the authority record is created or they’re needed to differentiate, but otherwise they aren’t included, even if the person goes on to become very famous—we don’t go back and add dates once a heading is established. 

In some cases, a person gets established under the name used on their first published work, and then they go on to use a different name predominantly.  Generally, once a heading is established it isn’t changed (though it can be under some circumstances).  We’ll usually just add 400 fields as cross-references from any other forms of name that someone might search under.  

So all this is to say that the way someone is established in the authority file might not be ideal, but we have to use that form regardless. 

## Subject headings

Say you want to add a subject heading about cooking, and you vaguely remember that the word “Cookery” was used for this concept in the past.  You might search “Cookery, American,” and get the following result: 

![screenshot](https://user-images.githubusercontent.com/58087302/78275344-7d7b8f00-74df-11ea-96ce-2d17d9094d0a.png "Cookery subject heading 1")

Do not just copy the heading found in this list into your record!  You need to open up the authority record and make sure that (1) you’re choosing the authorized form (rather than a cross reference), and (2) the heading is actually for a subject and not something else.  The authority file also includes records for things like series headings, which might look like subjects but are actually not. 

The “References” button next to Cookery, American, is a clue that this is actually a cross-reference and not an authorized heading.  Clicking on this button will lead you to the authority record, which looks like this: 

![screenshot](https://user-images.githubusercontent.com/58087302/78275865-3346dd80-74e0-11ea-9436-a2c5207b0c2b.png "Cookery subject heading 2")

Thus, “Cooking, American” is the authorized heading, because it’s in the 150 field.  “Cookery, American” is a superseded form of the heading.   

It’s also okay to copy subject heading strings that you find in the UNC catalog.  For more complicated headings with subdivisions, this will be much easier than searching the authority file.

For instance:

- Roads—North Carolina—Mecklenburg County—Design and construction. 
- University of North Carolina (1793-1962)--Students--Photographs. 
