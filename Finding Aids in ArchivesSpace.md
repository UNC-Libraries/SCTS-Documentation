Created by Dawne Lucas in August 2025 (in progress)

# Creating Finding Aids in ArchivesSpace at UNC-Chapel Hill

These are instructions for creating finding aids using ArchivesSpace, Pipette, and ArcLight (Archy) at the Wilson Special Collections Library at UNC-Chapel Hill. This documentation is supplemental to the documentation provided by ArchivesSpace, and has been adapted for use at the Wilson Special Collections Library. Some of the procedures described in this documentation differ from procedures followed at other institutions. It is therefore important that you read these procedures carefully, even if you already have experience using ArchivesSpace.

# Overview

 - [Introduction: ArchivesSpace, ArcLight (Archy), and Pipette](#introduction-archivesspace-arclight-archy-and-pipette)
 - [ArchivesSpace Terminology](#archivesspace-terminology)
 - [Finding Aid Creation](#finding-aid-creation)
   - [Resource Record Structure](#resource-record-structure)
   - [Collection-level Fields and Notes](#collection-level-fields-and-notes)
     - [Basic Information](#basic-information)
     - [Languages](#languages)
     - [Dates](#dates)
     - [Extents](#extents)
     - [Finding Aid Data](#finding-aid-data)
     - [Revision Statements](#revision-statements)
     - [Related Accessions](#related-accessions)
     - [Agent Links](#agent-links)
     - [Subjects](#subjects)
     - [Notes](#notes)
       - [Abstract](#abstract)
       - [Processing Information](#processing-information)
       - [Biographical and Historical Note](#biographical-and-historical-note)
       - [Scope and Content](#scope-and-content)
       - [Restrictions to Access](#restrictions-to-access)
       - [Restrictions to Use](#restrictions-to-use)
       - [Copyright Notice](#copyright-notice)
       - [Preferred Citation](#preferred-citation)
       - [Acquisitions Information](#acquisitions-information)
       - [Separated Materials](#separated-materials)
     - [External Documents](#external-documents)
     - [Rights Statements](#rights-statements)
     - [Metadata Rights Declarations](#metadata-rights-declarations)
     - [Instances](#instances)
     - [Deaccessions](#deaccesions)
     - [Collection Management](#collection-management)
     - [Classifications](#classifications)
     - [User Defined](#user-defined)
   - [Adding Series, Subseries, and File Level Archival Objects](#adding-series-subseries-and-file-level-archival-objects)
   - [Revising Series, Subseries, and File Level Archival Objects](#revising-series-subseries-and-file-level-archival-objects)
   - [Finding Aid Publication Workflow](#finding-aid-publication-workflow)
   - [Finding Aid Checklist](#finding-aid-checklist)
  
   ***
   
# Introduction: ArchivesSpace, ArcLight (Archy), and Pipette

Here’s the very tl;dr summary of the difference between ArchivesSpace, ArcLight (Archy), and Pipette:

 - **ArchivesSpace:** Staff-only interface used to create finding aids.
   - Staff interface: https://aspace.lib.unc.edu:4433/
   - Login using your ONYEN password.
   - Don't have an account? Contact Dawne.
 - **ArcLight (Archy):** Public-facing interface used to display finding aids.
   - https://finding-aids.lib.unc.edu/
   - UNC's version of ArcLight was named "Archy" (ArcLight at UNC-Chapel Hill) by Library Software Applications Developer Dean Farrell. "Archy" is UNC-specific, and the name is not used by other institutions using ArcLight.
 - **Pipette:** Staff-only interface used to preview and publish finding aids in ArcLight.
    - Preview: https://finding-aids-qa.lib.unc.edu/admin
    - Contact Dawne if you need access.   
    - NB: Content published to ArcLight is tracked via Git/Sourcetree, but TS-Archival does not interact with it. 
    - This is a UNC-specific application.
     
Remember: these are merely new tools for creating and displaying finding aids and do not replace our best practices for archival description, including:

 - <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md">Descriptive Elements</a>
 - <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Style%20Guide.md">Style Guide</a>

# ArchivesSpace Terminology

ArchivesSpace comes with its own jargon that might be new to you. Here are some terms that you should learn to love:

 - **Archival object:** Unit of archival description, such as a folder title.
   - Archival objects map to components (```<c0x>```) in EAD. 
 - **Instances:** Instances link archival objects to their physical containers (container instance) or digital files (digital object). 
   - ArchivesSpace is not a digital content repository and does not store digital files (just as it doesn’t store physical boxes). Digital objects merely serve as a link between ArchivesSpace and CONTENTdm, the DCR, or anywhere else digitized content might be stored.
 - **Resource:** Another term for "collection." Finding aids are generated from ArchivesSpace resource records.

# Finding Aid Creation

> These workflows are new to us and might change over time as ArchivesSpace changes over time and as we become more familiar with how to use it. If you see something in the instructions below that appears incorrect or just isn’t working for you, please contact Dawne ASAP.
>
> Furthermore, these workflows document UNC-specific procedures and do not cover everything there is to know about ArchivesSpace. Additional ArchivesSpace documentation is available via the <a href="https://archivesspace.atlassian.net/wiki/spaces/ADC/pages/917045261/ArchivesSpace+Help+Center">ArchivesSpace Help Center</a>, accessible via your Confluence account. Links to the ArchivesSpace Help Center are occasionally listed in the documentation below.

We create finding aids in ArchivesSpace using resource records. Resource records provide a structure to archival description similar to that found in our legacy EAD templates. Most fields in a resource record map to an EAD field, allowing end users to download a structured PDF version of the finding aids and (for anyone who wants it) the XML encoding. 

There are two ways to create resource records in ArchivesSpace. One way is to create a resource record within the Resource module. The other way is to "spawn" a resource record from an existing accession record. Both ways are subject to the same record requirements.

NB: Since we are using ArcLight instead of the ArchivesSpace Public User Interface, edits made to resource records will not automatically appear to the public. However, lengthy edits should be worked on outside of ArchivesSpace in order to avoid merge conflicts. More about that later!
 

## Resource Record Structure

Information in resource records is recorded in 18 different sections. You can see the sections listed in a menu on the left side of each resource record.

<img width="1416" height="609" alt="Picture1" src="https://github.com/user-attachments/assets/c4738500-624a-4c9c-8330-45cb13d27c8a" />

 - **1.	Basic Information:** As the name suggests, this is where basic information about the collection, such as collection title and collection number are recorded.
 - **2.	Languages:** The languages and scripts represented in the material(s) described.
 - **3.	Dates:** The dates(s) represented in the material(s) described.
 - **4.	Extents:** The size of the materials described.
 - **5.	Finding Aid Data:** Information about the finding aid, as opposed to the materials described.
 - **6.	Revision Statements:** Description(s) of revision(s) made to the finding aid.
 - **7.	Related Accessions:** Used for linking associated accessions to the resource record.
 - **8.	Agent Links:** Used for linking agent (name) records to the resource record.
 - **9.	Subjects:** Used for linking subject records to the resource record.
 - **10.	Notes:** This is where you enter all of various collection-level notes, including the Scope and Content note and the Biographical and Historical note. 
 - **11.	External Documents:** Links to pertinent information stored outside of ArchivesSpace, such as appraisal reports and spreadsheets. These will not display in the finding aid.
 - **12.	Rights Statements:** Used to record information about the rights status of the material being described.
 - **13.	Metadata Rights Declarations:** Used to record rights statement for archival description and archival authority records.
 - **14.	Instances:** Used to link containers (boxes, etc.) and information about digitized content.
 - **15.	Deaccessions:** Used to record information about materials that have been deaccessioned from the collection.
 - **16.	Collection Management:** Internal-only information about how the materials described will be or have been processed.
 - **17.	Classifications:** We are using classifications to record collecting units. This field allows faceting by collecting unit in ArcLight. Finding aids without an assigned classification cannot be published in ArcLight.
 - **18.	User Defined:** These fields are for internal purposes only. They do not display in ArcLight.

We will discuss each one of these sections in more detail later in this documentation. First, let’s discuss the fields that must be filled out in order to create a collection level record (CLR).

## Collection-level fields and notes

All resource records must have the following data, which contain red asterisks in ArchivesSpace:

 - Title
 - Identifier (a.k.a. Collection Number)
 - Level of Description (defaults to "Collection")
 - Languages sub-record
 - Date sub-record
 - Extents sub-record
 - Finding Aid Data ("Language of Description" and "Script of Description")
   
Resource records will not save unless these fields have been filled out. You should not add series, subseries, folders, boxes, etc., until these fields have been filled out.

Let’s go through each section of the collection level resource record. **Please note that except for the six fields listed above, you do not need to add all this information to a resource record at once.** 

You'll notice some fields in ArchivesSpace that aren't mentioned in these instructions. Rest assured that you don't have to worry about them.

When applicable, the EAD tags that fields map to are included in these instructions. This information is useful to staff members who have used EAD in the past. Don’t worry about them if you’re not familiar with EAD.

### Basic Information

<img width="693" height="320" alt="Picture2" src="https://github.com/user-attachments/assets/0a550fd0-4989-414c-b4f8-6955652859a5" />

 - **Title:** Collection title.
   - **Maps to:** ```<unittitle>```
   - **Example**: G. K. Butterfield Papers, 1942-2021
   - **Required to save record**
   - Note: Include the date, even though you will repeat it in the "Date" sub-record.

 - **Identifier:** Collection number. This number must be unique. You cannot create more than one resource record with the same identifier.
   - **Maps to:** ```<unitid>```
   - **Example:** 60010
   - **Required to save record**

- **Automatically Generate Slug?:** This box should already be checked.

- **Level of Description:** This value is automatically set to "Collection." If needed, you can change this value from the drop menu, although "Collection" should almost always suffice.
  - **Maps to:** ```<archdesc>```
  - **Required to save record**

- **Resource Type:** Select "Collection," "Papers," or "Records" from the drop menu, as appropriate.
  - Generally speaking, SFC = "Collection"; SHC = "Papers"; UARMS = "Records"

 - **Publish?:** This box needs to be checked in order for the finding aid to be indexed and published in ArcLight, including previewing on finding-aids-qa.

 - **Restrictions Apply?**: Check this box if the collection has any access or use restrictions.

 - **Repository Processing Note:** This is an optional field to record internal notes. It will not be seen by the public, even if the record is published.

### Languages 
Maps to: ```<langmaterial>```

 - **Language:** The language(s) represented in the materials. This value is automatically set to "English." This is usually correct!
   - **Maps to:** ```<langmaterial><language>```
   - **Required to save record**
   - For the small number of times when the default is not adequate, you can do one of the following: 
   - Change the language from "English" to whatever the appropriate language is. 
   - Add additional languages/scripts using the "Add Language" button available in the top right corner OR the bottom of the "Languages" section. You might have to hover to see the button at the bottom.


<img width="690" height="300" alt="Picture3" src="https://github.com/user-attachments/assets/ef1fdd00-06e4-450f-9aeb-2d0025dbcd55" />

 - **Language of Materials Note**: This value is automatically set to "Materials in English." This is usually correct!
   - **Maps to:** ```<langmaterial><language>```
   - For the small number of times when the default is not adequate, you can change the language from “English” to whatever the appropriate language(s) is/are.
  
 - **Script:** The script(s) represented in the materials (i.e., Latin, Gothic, Greek, etc.). This value is automatically set to "Latin." This is usually correct!
   - **Maps to:** ```<language>```
   - For the small number of times when the default is not adequate, you can change the script from “Latin” to whatever the appropriate script is.
  
### Dates

Maps to: ```<unitdate>```

<img width="698" height="242" alt="Picture4" src="https://github.com/user-attachments/assets/38630575-ed31-41ab-9a5a-a4eaf5ba5075" />

 - **Label:** This field defaults to "Creation," but can be changed via the drop menu if needed.
   - Required to save record
  
- **Expression:** The date or date range.
  - **Typically maps to:** ```<unitdate type="inclusive">```
  - Required to save record if the "Begin" and "End: fields are blank (see below). It is strongly recommended that you fill out the "Expression" field in addition to the "Begin" and "End" dates.
  - **Examples:**
    - 1985
    - November 1985
    - 1985-1990
    - circa 1985

- **Type:** This field defaults to "Inclusive," but can be changed via the drop menu if needed.
  - Required to save record.
 
 - **Begin and End:** Use these fields to record normalized dates.
  - **Maps to:** ```<unitdate type="normal">```
  - Required to save record if the “Expression” field is blank (see above). It is strongly recommended that you fill out the “Begin” and “End” dates as well as the “Expression” field.
  - Record single dates in the “Begin” field and leave the “End” field blank.
  - **Examples:**
    - 1985
      - Record in “Begin” field and leave “End” field blank.
    - 1985-1990
      - Record 1985 in the “Begin” field and 1990 in the “End” field.
        
**Pro tip:** You can add a bulk date by clicking the “Add Date” button in the top right corner OR the "+" at the bottom of the "Dates" section. You might have to hover to see the "+" at the bottom. Select "Bulk Date" for the "Type.”" 

**Note:** It's important to add the date, even though you are also recording the date in the “Title” field under “Basic Information.” 
  

### Extents

Maps to: ```<extent>```

<img width="714" height="242" alt="Picture5" src="https://github.com/user-attachments/assets/46e8c1d6-acad-4c88-a443-01824b237247" />

 - **Portion:** This field defaults to "Whole," but can be changed to "Part" via the drop menu if needed.
   - Required to save record.

- **Number:** The extent of the collection. It does not have to be a whole number.
  - Required to save record.
  - To be consistent with the nearly 6,200+ finding aids ingested into ArchivesSpace, it is strongly recommended to record the number of items in this field.
    - **Examples:**
      - 1
      - 3600
  

 - **Type:** Recommend setting to "items," but other values can be used as needed (say, "Gigabytes" if the collection is digital only).
   - Required to save record.
  
- **Container Summary:** Add additional extent information here. This will usually be the number of linear feet.
  - **Example:** 0.5 linear feet
  - Not required to save record, but strongly suggested to <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#extent">conform to our practices.</a> 


**Pro tip:** You can add more extents by clicking the "Add Extent" button in the top right corner OR the "+" at the bottom of the "Extents" section. You might have to hover to see the "+" at the bottom.  Select "Part" for the "Portion." 

### Finding Aid Data

Maps to: ```<eadheader>```

Information in these fields will not be seen by the public, even if the rest of the record is published. 

<img width="707" height="367" alt="Picture6" src="https://github.com/user-attachments/assets/29ee8188-392d-4033-b576-da6278890e7c" />

You can ignore any field not mentioned below.

- **EAD ID:** The EAD ID is the same as the collection number. 
  - **Maps to:** ```<eadid>```
  - Not required to save record, **but please do fill it out.** You cannot upload spreadsheets or index in Archy without this field (more on that later).
  - **Example:** 60010

- **Finding Aid Title:** The Finding Aid Title is the same as the collection title.
  - **Maps to:** ```<titleproper>```
  - **Example:** Dawne Howard Lucas Papers

- **Finding Aid Date:** The date the finding aid was completed.
  - **Maps to:** ```<profiledesc><creation>```
  - **Example:** August 2021
 
- **Finding Aid Author:** The name of the person who completed the finding aid.
  - **Maps to:** ```<profiledesc><creation>```
  - **Example:** Nancy Kaiser
 
 - **Description Rules:** Please don’t populate this field. At the moment it causes display issues in Archy.

 - **Language of Description Note:** This field defaults to "English." Unless you are creating a finding aid in another language (unlikely!), you will never need to change this default.
   - **Maps to:** ```<langusage><language>```
   - Required to save record

- **Sponsor:** This field will usually be blank. It can be used to record sponsor information when applicable.
  - **Maps to:** ```<sponsor>```
  - **Example from finding aid ingested from EAD:** Funding from the State Library of North Carolina supported the encoding of this finding aid. Funding from the Terry and Laurie Sanford Library Fund supported the digitization of this collection.
 
- **Finding Aid Status:** Use the drop menu to choose the correct status. Make sure to set it to "Completed" once it is done!
  - **Maps to:** ```<eadheader findaidstatus>```
  - If working on a new finding aid, use the status "In Progress." When a resource record is set to this status, it cannot be published via Pipette.
  - If revising an existing finding aid, use the status "Under Revision." When a resource record is set to this status, it cannot be published via Pipette.
  - Make sure to set the status to "Completed" once you are done! Changing the status will allow the resource record to be published via Pipette.
 
- **Finding Aid Status Published?:** This box should remain unchecked.

- **Finding Aid Note:** You can use this note to record any extraneous internal information about the finding aid. Remember, these notes will not be seen by the public. 
  - **Maps to:** ```<notestmt>```
  - For finding aids ingested from EAD, this field is populated with "This finding aid is NCEAD compliant."
    
### Revision Statements

Maps to: ```<revisiondesc>```

This field is also part of the ```<eadheader>``` and will not be seen by the public, even if the rest of the record is published. But it's still very important!
When you revise a resource record, add a Revision Statement by clicking the "Add Revision Statement" button.

You will then see the following fields:

- **Revision Date:** The date the revisions were made. You can use this format: ```MONTH YEAR```
  - Required to save record.
  - **Example:** August 2025

- **Revision Description:** An explanation of who made the revision and why.
  - Required to save record
  - **Example:** Revised by Jodi Berkowitz to correct biographical information.

- **Publish?:** Since this field won’t display regardless, there’s no need to worry about this box.

<img width="711" height="165" alt="Picture7" src="https://github.com/user-attachments/assets/a7364b7b-fb0c-4f18-a651-b9136975df66" />

**Pro tip:** You can add more Revision Statements by clicking the "Add Revision Statement" button in the top right corner OR the "+" at the bottom of the "Revision Statements" section. You might have to hover to see the "+" at the bottom.  

### Related Accessions

This field will list any accessions linked to this resource record. These links do not appear in the published finding aid in Archy. They are usually linked from the accession record, so you shouldn't have to do anything here.

<img width="751" height="127" alt="Picture8" src="https://github.com/user-attachments/assets/22d561a4-a14a-45d2-bd74-9e20d8d6e0b4" />

IF you do need to link an accession record for some reason, click on the "Add Related Accession" button, search for the accession, and link it to the resource record. 

**Pro tip:** You can add more Related Accessions by clicking the "Add Related Accession" button in the top right corner OR the "+" at the bottom of the "Related Accessions" section. You might have to hover to see the "+" at the bottom. 

### Agent Links

Maps to: ```<origination>``` and ```<controlaccess>```

Agents are person (```<persname>```), family (```<famname>```) or corporate (```<corpname>```) names that are associated with the collection as creators or subject headings (geographic names are entered as Subjects).

**Pro tip:** You can add more Agents by clicking the "Add Agent Link" button in the top right corner OR the "+" at the bottom of the "Agent Links" section. You might have to hover to see the "+" at the bottom.

- **Role:** Select "Creator" or "Subject."
  - Required to save record
  - Agents linked with the "creator" role will appear as the creator (```<origination>```).
  - Agents linked with the "subject" role will appear in the finding aid's subject headings ```<controlaccess>```).
  - If an agent is both the creator and a subject, link it twice, once with the "creator" role and once with the "subject" role.

<img width="530" height="135" alt="Picture9" src="https://github.com/user-attachments/assets/07aa6c9d-b80a-44ec-9d95-f1e6ed6d1539" />

 - **Agents:**
   - Required to save record
   - To link an existing agent record, you can either begin typing in the name and select from a list of autocomplete options presented by ArchivesSpace OR use the "Browse" option.
     - Autocomplete:
      <img width="528" height="152" alt="Picture10" src="https://github.com/user-attachments/assets/0d2fcb70-0852-42bc-9eb6-da117aa40635" />
   - If using the "Browse" option, search for and select the desired agent, and then click "Link."
     - Browse:
       
        <img width="530" height="146" alt="Picture11" src="https://github.com/user-attachments/assets/15a74c45-3e9f-48a9-bb70-07021f5c12e0" />
        <img width="578" height="326" alt="Picture12" src="https://github.com/user-attachments/assets/61cb8694-7e96-4f7a-9f76-ce95fe2d9563" />
        
   - Many agent records that were ingested into ArchivesSpace from EAD are not formatted correctly. Don’t worry...they’re fine as they are right now.
  
   - To create a new agent record, select "Create" and then select the type of agent record you wish to create (Person, Family, or Corporate Entity). A minimal agent record may be created by filling in only the required fields. The minimal record can be enhanced later by adding additional information in other fields and sub-records. For more details about creating new agent records, visit the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/1942945864/Agent+Record+Fields+from+3.0">Agent Record Fields</a> page in the ArchivesSpace Help Center.
     
     - Create:
       
    <img width="530" height="197" alt="Picture13" src="https://github.com/user-attachments/assets/b57903b4-99b6-4340-8ef4-e40f2ad1c9f0" />
    
     - If an agent is listed in <a href="https://authorities.loc.gov/">LCNAF</a>, paste the "LCCN Permalink" in the "Authority ID" field.

### Subjects

Subjects (```<subject>```, ```<geogname>```, ```<genreform>```) are the finding aid's topical subject headings. Adding subject headings is similar to adding agent links.

**Pro tip:** You can add more Subjects by clicking the "Add Subject" button in the top right corner OR the "+" at the bottom of the "Subjects" section. You might have to hover to see the "+" at the bottom.

- **Subjects:**
  - Required to save record.
  - To link an existing subject record, you can either begin typing in the subject and select from a list of autocomplete options presented by ArchivesSpace OR use the "Browse" option.
  - If using the "Browse" option, search for and select the desired subject, and then click "Link."
  - Many subject records that were ingested into ArchivesSpace from EAD are probably not formatted correctly. Don’t worry...they’re fine as they are right now.
  - To create a new subject record, select "Create" and fill in the "Term" and "Type" fields. For more details about creating new subject records, visit the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/894664812/Subject+Record+Fields">Subject Record Fields</a> page in the ArchivesSpace Help Center.
    - If a subject heading is listed in <a href="https://authorities.loc.gov/">LCSH</a>, enter the "LCCN Permalink" in the "Authority ID" field.

To add personal, family, or corporate names as subject headings, see the "Agent Links" section above. For more details about creating new agent records, visit the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/1942945864/Agent+Record+Fields+from+3.0">Agent Record Fields</a> page in the ArchivesSpace Help Center.

### Notes

#### Abstract

> Required!

#### Processing Information

> Required!

#### Biographical and Historical Note

> Required!

#### Scope and Content

> Required!

#### Restrictions to Access

> Required! 

#### Restrictions to Use

> Delete if not needed.

#### Copyright Notice

> Required for NCC, RBC, SFC, and SHC. Delete for UARMS.

This note contains the following boilerplate text:

```Copyright is retained by the authors of items in these papers, or their descendants, as stipulated by United States copyright law.```

Unless otherwise specified in the accession record, you do not need to do anything to this field.


#### Preferred Citation

> Required!

This note contains the following boilerplate text:

```[Identification of item], in the [collection name and number], Wilson Special Collections Library, University of North Carolina at Chapel Hill.```

You do not need to do anything to this field.


#### Acquisitions Information

#### Separated Materials

### External Documents

Don’t worry about these fields, at least for right now. They can be used to link to information in other description management tools, such as donor files or processing plans. Maybe we’ll decide to use them in the future, but we’re not ready to experiment with it yet.

### Rights Statements

Don’t worry about these fields. We are not using them at this time.

### Metadata Rights Declarations

No need to worry about these fields. We are not using them at this time. Should we decide to start using them, the information will likely become part of the template that is automatically generated with new resource records.

### Instances

Instances refer to physical containers and digital objects.  **See Adding Series, Subseries, and File Level Archival Objects (below) for how to add instances to resource records.**

> *Please note the current workflow for adding instances to resource records differs from the workflow used during the ArchivesSpace implementation period (2020-2024). Please do not attempt to use the old workflow. Doing so will cause a lot of confusion in Archy and to our R&IS colleagues.*


### Deaccessions

These fields are used to record information about deaccessions, and should only be used by the Technical Services Archivist for Collection Management.

### Collection Management

Leave these fields blank. These fields are used to record processing information. Since we record this information on the accession records, this information does not need to be filled out here.

### Classifications

### User Defined

These fields are used to record additional information not accounted for in other fields. They are for internal purposes only and will not display in the finding aid.
At this time, we are using the following User Defined fields for resource records. More fields might be added in the future:

 - **Contains harmful content?:** Check this box if a collection contains materials with harmful content.
   - Examples:
    - Photographs of lynchings
    - Letters that contain hate speech
 - **Requestable?**
   - Check this box if materials should be requestable in Archy.
 - **Description of harmful content:** Use this box to describe the materials with harmful content. 
   - Examples:
     - Image folder 7 contains photographs of lynchings.
     - Folder 10 contains letters that contain racist language.


# Adding Series, Subseries, and File Level Archival Objects

# Revising Series, Subseries, and File Level Archival Objects

# Finding Aid Publication Workflow

# Finding Aid Checklist


